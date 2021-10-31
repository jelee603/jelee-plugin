<template>
  <div id="app">
    <img class="logo" alt="Vue logo" src="./assets/logo.png">
    <span>Echart Test</span>
    <ChartTest/>
    <img class="logo" alt="Vue logo" src="./assets/logo.png">
    <span>Table Slot include Custom Table</span>
    <Table />
  </div>
</template>

<script>
import ChartTest from './components/ChartTest.vue'
import Table from './components/Table.vue'

export default {
  name: 'App',
  components: {
    ChartTest,
    Table,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
}

.logo {
  width: 40px; 
  height: 40px;
}
</style>
