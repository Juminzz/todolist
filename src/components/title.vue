<template>
  <div id="title">
    <div>{{ today }}</div>
    <h1>{{ name }}</h1>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name: "Title",
  props: {
    name: String,
  },
  data() {
    return {
      today: new Date().toLocaleDateString(),
    };
  },
  methods: {},
};
</script>

<style></style>
