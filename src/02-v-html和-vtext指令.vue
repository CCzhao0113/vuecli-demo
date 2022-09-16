<template>
  <div>
    <p v-text="text"></p>
    <p v-html="html"></p>
  </div>
</template>

<script>
export default {
  //指令的优先级要高于插值语法
  //v-text和原生的innerText一样
  // v-html和原生的innerHTML一样
data(){
  return{
    text:'这是一个v-text指定渲染的文本',
    html:'<h1>这是一个v-html指令渲染的文本</h1>'
  }
}
}
</script>

<style>

</style>