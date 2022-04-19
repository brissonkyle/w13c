<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <PageComp/>
  </div>
</template>

<script>
import PageComp from './components/PageComp.vue'


export default {
  name: 'App',
  components: {
    PageComp,
  }
}
</script>

<style lang="scss">
html {
  background-color: violet;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
