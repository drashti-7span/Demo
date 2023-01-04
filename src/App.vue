<template>
  <div id="app">   
    <TheHome date="Hello World" msg="Hello 2"/>
    <TheAbout />
    <DataBind />
    <TheChild name="Anil Shidhu"/>
  </div>
</template>
<script>

import TheHome from './components/TheHome.vue'
import TheAbout from './components/TheAbout.vue'
import DataBind from './components/DataBind.vue'
import TheChild from './components/TheChild.vue'
export default {
  name: 'App',
  components: {
    TheHome,
    TheAbout,
    DataBind,
    TheChild
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
