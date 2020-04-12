<template>
  <div id="app">
    <HelloImasWorld />
  </div>
</template>

<script>
import HelloImasWorld from './components/HelloImasWorld.vue'

export default {
  name: 'App',
  components: {
    HelloImasWorld
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
