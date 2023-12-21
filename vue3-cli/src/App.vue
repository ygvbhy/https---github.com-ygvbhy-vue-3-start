<template>
  <AppHeader :appTitle="message" @change="changeAppTitle" />
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
export default {
  components: {
    // 축약 과정
    // 'app-header': AppHeader => 케밥 케이스
    // 'AppHeader': AppHeader => 카멜 케이스
    // AppHeader: AppHeader => 파스칼 케이스 -> 이걸로 쓰는걸 추천함.
    AppHeader,

    // 번외 -> app_header => 스네이크케이스
  },
  data() {
    return {
      message: "App Header Component",
    };
  },
  methods: {
    changeAppTitle() {
      this.message = "변경됨";
    },
  },
};
</script>

<style scoped></style>
