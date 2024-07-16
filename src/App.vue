<script>
import Calculator from './components/Calculator.vue';

export default {
  name: 'App',
  components: {
    Calculator,
  },
};
</script>

<template>
  <div id="app">
    <Calculator />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
* {
  background-color: #666666;
  color: white;
  border-color: white;
  font-weight: bold;
}
</style>
