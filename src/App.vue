<template>
  <div>
    <h1>{{msg}}</h1>
    <button @click="click">逆转</button>
  </div>
</template>

<script>
export default {
data() {
  return {
    msg: 'Hello World',
  };
},
methods:{
  click(){
 const arr = this.msg.split('')
 const newArr = arr.reverse()
 this.msg = newArr.join('')
  }
}
}
</script>

<style>

</style>