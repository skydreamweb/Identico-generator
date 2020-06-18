<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/identico.png">
    <Input msg="Welcome to Identico App"/>
    <Output></Output>
  </div>
</template>

<script>
import Input from './components/Input.vue'
import Output from './components/Output.vue'

export default {
  name: 'App',
  components: {
    Input,
    Output
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
