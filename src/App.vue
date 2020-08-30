<template>
  <div id="app">
    <Todos v-bind:todos="todos" v-on:del-todo="deleteTodo" />
  </div>
</template>

<script>
import Todos from "./components/Todos";

export default {
  name: "App",
  components: {
    Todos,
  },

  data() {
    return {
      todos: [
        {
          id: 1,
          title: "Morning priming",
          completed: true,
        },
        {
          id: 2,
          title: "Practicing algorithms and data structures",
          completed: false,
        },
        {
          id: 3,
          title: "Create and work on new Websocket project",
          completed: false,
        },
        {
          id: 4,
          title: "Gym",
          completed: false,
        },
      ],
    };
  },
  methods: {
    deleteTodo(id) {
      this.todos = this.todos.filter((todo) => todo.id !== id);
    },
  },
};
</script>

<style>
</style>
