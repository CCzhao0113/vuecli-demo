<template>
  <div>
    <a href="http://www.baidu.com" @click.prevent="clickFn">去百度</a>
    <input type="text" @keydown="keyFn">
    <input type="text" @keydown.ctrl="enterFn">
  </div>
</template>

<script>
export default {
methods:{
  clickFn(){
    // e.preventDefault()
  },
  keyFn(){
    console.log('an下了键盘');
  },
  enterFn(){
    console.log('an下了键盘enter');
  }
}
}
</script>

<style>

</style>