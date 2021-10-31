<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" style="width: 40px; height: 40px">
    <span>Echart Test</span>
    <ChartTest/>
  </div>
</template>

<script>
import ChartTest from './components/ChartTest.vue'

export default {
  name: 'App',
  components: {
    ChartTest,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
