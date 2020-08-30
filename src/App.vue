<template>
  <div id="app"></div>
</template>

<script>
export default {
  name: "App",
  components: {},
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
