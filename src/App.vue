<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <h1>Responsive Chart Plot Line Using a Pure HTML and CSS</h1>
    <Axis />
  </div>
</template>

<script>
import Axis from "./components/Axis.vue";

export default {
  name: "App",
  components: {
    Axis
  }
};
</script>

<style>
body {
  background-color: #2c3e50;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: azure;
  margin-top: 60px;
}
</style>
