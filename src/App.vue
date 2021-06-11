<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <AlanRails/>
    <Character/>
    <Character/>
  </div>
</template>

<script>
import AlanRails from './components/AlanRails.vue'
import Character from './components/Character.vue'
export default {
  name: 'App',
  components: {
    AlanRails,
    Character
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
