<template>
  <div>
    <a :href="hrefStr" @click="clickFn">去百度</a>
    <a :href="hrefStr" @click="clickFn1(10,$event)">去百度</a>
  </div>
</template>

<script>
export default {
data() {
  return {
    hrefStr: 'http://www.baidu.com',
  }
  
},
methods:{
clickFn(e){
  console.log(e);
  e.preventDefault()
},clickFn1(e ,ev){
  console.log(e);
  ev.preventDefault()
}
}
}
</script>

<style>

</style>