<template>
  <form action="">
    <div>
      <label for="userId">ID:</label>
      <input type="text" id="yserID" v-model="username" />
    </div>
    <div>
      <label for="password">PW:</label>
      <input type="password" id="password" v-model="password" />
    </div>
    <button type="submit">로그인</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      username: "",
      password: "",
    };
  },
};
</script>

<style scoped></style>
