<template>
  <div id="app">
    <img src="./assets/logo.png">
    <Demo></Demo>
    <router-view/>
  </div>
</template>

<script>
// 导入其它组件
import Hello from './components/HelloWorld'
import Demo from './components/Demo'
export default {
  name: 'App', // 当前vue的文件名称
  components: {
    Hello,
    Demo
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
