<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from "./components/Todos";
export default {
  name: "App",
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        { id: 1, title: "Just a task", completed: false },
        { id: 2, title: "complete Vue JS", completed: true },
        { id: 3, title: "Host my app", completed: false },
        { id: 4, title: "Open a mail account", completed: true }
      ]
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
