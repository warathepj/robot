<template lang="">
  <div class="card">
    <h1>{{ emoji }}</h1>
    <div class="content">
      <p>{{ p1 }}</p>
      <h6>{{ h6 }}</h6>
      <p>{{ p2 }}</p>
      <p>{{ p3 }}</p>
    </div>
    <button
      :style="{ backgroundColor: hoverColor }"
      @mouseover="onHover"
      @mouseleave="onLeave"
    >
      {{ text }}
    </button>
  </div>
</template>
<script>
export default {
  name: "Button",
  props: {
    label: String,
    style: Object,
    emoji: String,
    p1: String,
    h6: String,
    p2: String,
    p3: String,
    btnTxt: String,
    btnColor: String,
    text: String,
    hoverColor: String,
  },
  methods: {
    handleClick() {
      this.$emit("click");
    },
    onHover() {
      this.$emit("hover");
    },
    onLeave() {
      this.$emit("leave");
    },
  },
};
</script>
<style scoped>
.card {
  background: rgb(178, 143, 247);
  color: black;
  display: flex;
  flex-direction: row;
  align-items: center;
  margin: 0 20px 20px 0;
  border-radius: 10px;
  padding: 0.6rem;
}
.content {
  line-height: 0.2;
}
h1 {
  padding: 0 5px 0 6px;
}
button {
  width: 5rem;
  height: 1.3rem;
  border-radius: 0.4rem;
}
</style>
