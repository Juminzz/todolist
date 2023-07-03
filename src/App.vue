<template>
  <Title id="todo" name="To-Do-List" />
  <todoinput />
  <todolist />
</template>

<script>
/* eslint-disable */
import Title from "./components/title.vue";
import todoinput from "./components/input.vue";
import todolist from "./components/todolist.vue";

export default {
  name: "App",
  components: {
    Title,
    todoinput,
    todolist,
  },
  data() {
    return {
      todos: [],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}
#todo {
  font-weight: bold;
  text-decoration: none;
  color: #42b983;
  font-size: 20px;
}
</style>
