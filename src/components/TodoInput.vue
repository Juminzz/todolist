<template>
  <div>
    <input type="text" v-model="newTodoItem" v-on:keyup.enter="addTodo" />
    <button @click="addTodo">add</button>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name: "app",
  data: function () {
    return {
      newTodoItem: "",
    };
  },
  methods: {
    addTodo: function () {
      console.log(this.newTodoItem);
      // 저장하는 로직
      localStorage.setItem(this.newTodoItem, this.newTodoItem);
      this.newTodoItem = ""; // 초기화
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Itim&display=swap");
html,
body {
  font-family: "Itim", cursive;
}
#app {
  font-family: "Itim", cursive;
}
</style>
