<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <CustomCheckBox/>
  </div>
</template>

<script>
import CustomCheckBox from './components/CustomCheckBox.vue'

export default {
  name: 'App',
  components: {
    CustomCheckBox
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
