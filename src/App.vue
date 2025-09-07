<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <h1>Hello {{ name }}, I hear this is your first Vue.js app!</h1>
  <div>{{ course }} Year 4</div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Nanak",
      course: "Computer Science",
    };
  },
};
</script>

<style>
#app {
  font-family: Outfit, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
