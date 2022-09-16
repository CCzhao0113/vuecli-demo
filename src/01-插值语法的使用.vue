<template>
  <!-- 在vue中有且只能有一个根元素 -->
  <div>
    <p>姓：{{username}}名：{{username1()}}</p>
    <!-- 使用数据，在template中可以直接使用data中定义好的数据 -->
    <p>{{age > 18? '成年了':'未成年'}}</p>
  </div>
</template>

<script>
  //核心思想：数据驱动视图
export default {
//data是一个函数，用来存放数据
//里面必须要有return
data (){
  return {
    //准备数据，以键值对的形式存放数据
    //name在谷歌调试工具中文件的名字
    name :'app',
  username:"赵",
  username1:function(){
    return 1+1
  },
  age:19
  }
}
}
</script>

<style>

</style>
