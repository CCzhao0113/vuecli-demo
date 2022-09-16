<template>
  <div>
    <p>{{ num }}</p>
    <!-- 如果事件逻辑比较简单，也可以直接对data中的数据进行操作进而使得页面发生变化 -->
    <button v-on:click="clickFn">点击+1</button>
    <button v-on:click="num++">点击+1</button>
    <button v-on:click="clickFn1">点击-1</button>
    <button v-on:click="num--">点击-1</button>
    <button v-on:click="click(10)">点击+10</button>
    <button @click="click1(10)">点击-10</button>
    <button @mouseenter="click1(10)">点击-10</button>
  </div>
</template>

<script>
export default {

data() {
  return {
    num: 0,
  };
},
methods:{
  clickFn(){
    this.num++
  },
  clickFn1(){
    this.num--
  },
  click(value){
    this.num +=value
  },
  click1(value){
    this.num -=value
  }
  
}
}
</script>

<style>

</style>