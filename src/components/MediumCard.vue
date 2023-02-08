<template lang="">
  <div class="medium-card">
    <h4 class="robot">🤖</h4>
    <article>
      <p>Lorem ipsum</p>
      <p>dolor, sit amet consectetur adipisicing elit.</p>
    </article>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.medium-card {
  background: linear-gradient(to top right, #5162f8, #d145fc);
  width: 125px;
  height: 145px;
  padding: 6px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
}
.robot {
  margin: 0 0 0 0;
  font-size: 2rem;
}
article {
  margin-top: -5px;
}
article p:first-of-type {
  font-size: 1.2rem;
  margin-bottom: -10px;
}
p {
  font-size: 1rem;
}
</style>
