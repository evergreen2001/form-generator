<template>
  <div id="app">
    
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
