<template>
  <div id="app">{{myName}}</div>
</template>

<script>
export default {
  name: "App",
  components: {},
  data() {
    return {
      myName: "Kaiser Phemi"
    };
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
