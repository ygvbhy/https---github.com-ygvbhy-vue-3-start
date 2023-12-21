<template>
  <h1>{{ appTitle }}</h1>
  <button @click="changeTitle">바꾸기</button>
</template>

<script>
export default {
  props: {
    appTitle: {
      type: String,
      default: "",
    },
  },
  methods: {
    changeTitle() {
      this.$emit("change");
    },
  },
};
</script>

<style scoped></style>
