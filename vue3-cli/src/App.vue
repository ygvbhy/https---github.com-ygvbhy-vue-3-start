<template>
  <AppHeader />
  <div>{{ message }}</div>
  <button @click="showAlert">경고</button>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
export default {
  components: {
    // 축약 과정
    // 'app-header': AppHeader => 케밥 케이스
    // 'AppHeader': AppHeader => 카멜 케이스
    // AppHeader: AppHeader => 파스칼 케이스
    AppHeader,

    // 번외 -> app_header => 스네이크케이스
  },
  data() {
    return {
      message: "hi",
    };
  },
  methods: {
    showAlert() {
      alert("hello");
    },
  },
};
</script>

<style scoped></style>
