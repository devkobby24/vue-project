<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <h1 v-bind:style="{ color: color, fontSize: fontSize }">
    Hello {{ name }}, I hear this is your first Vue.js app!
  </h1>
  <div v-html="course"></div>
  <h2
    v-bind:class="isDangerous ? 'danger' : 'safety'"
    v-text="isDangerous ? text : text1"
  ></h2>
  <button v-bind:disabled="isDisabled">Submit Me!</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Nanak",
      headingClass: "heading-1",
      isDisabled: true,
      isDangerous: false,
      status: "danger",
      text: "Danger",
      text1: "We are safe",
      color: "blue",
      fontSize: "48px",
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

.heading-1 {
  font-size: 24px;
  color: #42b983;
  margin-bottom: 20px;
  font-weight: bold;
}

.danger {
  color: white;
  background-color: red;
  width: 100px;
  margin: 0 auto;
  padding: 10px;
  border-radius: 10px;
}
.safety {
  color: white;
  background-color: green;
  width: 100px;
  margin: 0 auto;
  padding: 10px;
  border-radius: 10px;
}
</style>
