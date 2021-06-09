<template>
  <div id="app">
    <Main />
    <Mastercraft />
    <Number />
  </div>
</template>

<script>
import Main from './components/Main'
import Mastercraft from './components/Mastercraft.vue'
import Number from './components/Number.vue'

export default {
  name: 'App',
  components: {
    Main,
    Mastercraft,
    Number
  }
}
</script>

<style>
*{margin:0;padding:0;}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background:rgb(230, 230, 230)
}
</style>
