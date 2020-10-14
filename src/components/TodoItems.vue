<template>
  <div class="todo-item" v-bind:class="{ 'is-complete': todo.completed }">
    <p>
      <input type="checkbox" v-on: cha
      {{ todo.title }}
    </p>
  </div>
</template>

<script>
export default {
  name: "TodoItem",
  props: ["todo"],
};
</script>

<style scoped>
.todo-item {
  background: #f4f4f4;
  padding: 1em;
  border: 1px grey solid;
}

.is-complete {
  text-decoration: line-through;
}
</style>
