<template>
  <div id="app">
    <Header />
    <AddTodo v-on:add-todo="addTodo" />
    <Todos v-bind:todos="todos" v-on:del-todo="deleteTodo" />
  </div>
</template>

<script>
import Header from './components/layout/Header';
import Todos from './components/Todos';
import AddTodo from './components/AddTodo';

export default {
  name: 'App',
  components: {
    Header,
    Todos,
    AddTodo,
  },

  data() {
    return {
      todos: [
        {
          id: 1,
          title: 'Morning priming',
          completed: true,
        },
        {
          id: 2,
          title: 'Practicing algorithms and data structures',
          completed: false,
        },
        {
          id: 3,
          title: 'Create and work on new Websocket project',
          completed: false,
        },
        {
          id: 4,
          title: 'Gym',
          completed: false,
        },
      ],
    };
  },
  methods: {
    deleteTodo(id) {
      this.todos = this.todos.filter((todo) => todo.id !== id);
    },
    addTodo(newTodo) {
      this.todos = [...this.todos, newTodo];
    },
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.btn {
  display: inline-block;
  border: none;
  background: #555;
  color: #fff;
  padding: 7px 20px;
  cursor: pointer;
}
.btn:hover {
  background: #666;
}
</style>
