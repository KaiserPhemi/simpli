<template>
  <div class="td-item">
    <input type="checkbox" name="completed" class="completed" v-on:change="markComplete" />
    <span v-bind:class="{'is-completed':todo.completed}">{{todo.title}}</span>
  </div>
</template>

// main script
<script>
export default {
  name: "TodoItem",
  props: ["todo"]
};
</script>

// Styles
<style scoped>
.td-item {
  align-items: center;
  border: 1px solid #bada55;
  border-radius: 5px;
  cursor: pointer;
  display: grid;
  grid-template: 1fr / 1fr 7fr;
  margin: 1rem auto;
  padding: 10px;
  width: 20%;
}

.is-completed {
  text-decoration: line-through;
}

.item {
}

.completed {
  cursor: pointer;
}
</style>