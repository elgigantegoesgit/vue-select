<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <selectexample msg="simple vue-select example with vue 3" />
</template>

<script>
import selectexample from "./components/selectexample.vue";

export default {
  name: "App",
  components: {
    selectexample: selectexample,
  },
};
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
