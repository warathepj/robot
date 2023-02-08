<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <div class="wrapper">
    <h3>🔥 Lorem ipsum</h3>
    <div class="container">
      <div class="nav">
        <RouterLink to="/" class="tdn">Home</RouterLink>
        <RouterLink to="/about" class="tdn">About</RouterLink>
        <RouterLink to="/dolor" class="tdn">Dolor</RouterLink>
        <RouterLink to="/sit" class="tdn">Sit</RouterLink>
      </div>
      <div class="login">
        <RouterLink to="/login" class="tdn">Log in</RouterLink>
        <RouterLink to="/signup" class="tdn">Sign up</RouterLink>
      </div>
    </div>
  </div>
  <RouterView />
</template>

<style scoped>
.wrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  column-gap: 40px;
}

.nav {
  margin-top: 25px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  column-gap: 10px;
}
.tdn {
  height: 1.4rem;
  width: 80px;
  padding: 1px;
  text-decoration: none;
  text-align: center;
  color: white;
}
.tdn:hover {
  background: #0652dd;
}
.login {
  margin-top: 25px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  column-gap: 10px;
}
</style>
