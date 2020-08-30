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
    Todos,
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "Morning priming",
          completion: true,
        },
        {
          id: 2,
          title: "Practicing algorithms and data structures",
          completion: false,
        },
        {
          id: 3,
          title: "Create and work on new Websocket project",
          completion: false,
        },
        {
          id: 4,
          title: "Gym",
          completion: false,
        },
      ],
    };
  },
};
</script>

<style>
</style>
