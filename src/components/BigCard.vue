<template lang="">
  <div class="big-card">
    <div class="wrapper">
      <div class="big-font">
        <h1>Lorem ipsum dolor sit</h1>
      </div>
      <p class="p1">
        amet consectetur adipisicing elit. Ad debitis at consectetur eum dolores
        assumenda hic
      </p>
      <img src="../assets/no-bg.png" alt="" />
      <div class="content">
        <h1>AI</h1>
        <h3>tempore expedita, tenetur error in? Eius in molestiae,</h3>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.big-card {
  background: #0652dd;
  margin-top: 0px;
  padding: 5px 40px 5px 40px;
  border-radius: 30px;
}
.big-font {
  width: 13vw;
  font-size: 1.9rem;
  line-height: 0.9;
  background: -webkit-linear-gradient(#fae9e9, #6d6ffa);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.wrapper {
  display: flex;
  flex-direction: row;
}
.p1 {
  width: 85px;
  font-size: 0.8rem;
  margin: 50px 0 0 16px;
  color: rgb(178, 143, 247);
}
img {
  height: 350px;
  margin: -60px 0px 0 70px;
}
.content {
  width: 10rem;
  display: flex;
  flex-direction: column;
}
</style>
