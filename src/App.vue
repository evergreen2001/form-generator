<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <FormPage/>
  </div>
</template>

<script>
import FormPage from './components/FormPage.vue'

export default {
  name: 'App',
  components: {
    FormPage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin-top: 60px;
}
</style>
