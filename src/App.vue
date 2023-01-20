<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <TestComponent />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TestComponent from "./components/TestComponet.vue";

export default {
  name: "App",
  components: {
    TestComponent,
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
