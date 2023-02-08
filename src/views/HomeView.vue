<script>
import BigCard from "../components/BigCard.vue";
import SmallCard from "../components/SmallCard.vue";
import MediumCard from "../components/MediumCard.vue";

export default {
  data() {
    return {
      width: 240,
      button1HoverColor: "red",
      button2HoverColor: "blue",
    };
  },
  components: {
    BigCard,
    SmallCard,
  },
  methods: {
    onButton1Hover() {
      this.button1HoverColor = "yellow";
    },
    onButton1Leave() {
      this.button1HoverColor = "red";
    },
    onButton2Hover() {
      this.button2HoverColor = "green";
    },
    onButton2Leave() {
      this.button2HoverColor = "blue";
    },
  },
};
</script>

<template>
  <main>
    <div class="big-card">
      <BigCard />
    </div>
    <div class="small-card">
      <SmallCard
        :emoji="'💀'"
        :p1="'Lorem ipsum'"
        :h6="'99.8dolor'"
        :p2="'consectetur'"
        :p3="'adipisicing elit.'"
        :btnTxt="'error'"
        :btnColor="'red'"
        text="Button 1"
        :hoverColor="button1HoverColor"
        @hover="onButton1Hover"
        @leave="onButton1Leave"
      />
      <SmallCard
        :emoji="'✨'"
        :p1="'Natus inventore'"
        :h6="'115dolor'"
        :p2="'obcaecati'"
        :p3="'soluta eum'"
        :btnTxt="'quasi'"
        :btnColor="'blue'"
        text="Button 2"
        :hoverColor="button2HoverColor"
        @hover="onButton2Hover"
        @leave="onButton2Leave"
      />
    </div>
    <div class="container">
      <img
        src="https://images.unsplash.com/photo-1517336714731-489689fd1ca8?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=200&q=80"
        alt=""
      />
      <div class="half-cir">
        <h3>SIT AMET CONSECTETUR ADIPISICING</h3>
      </div>
      <div class="content1">
        <p>
          <span>Lorem ipsum</span> dolor, sit amet consectetur adipisicing elit.
        </p>
        <MediumCard />
      </div>
      <div class="container2">
        <div class="content2">
          <svg width="120" height="70">
            <circle cx="20" cy="20" r="10" fill="blue" />
            <circle cx="90" cy="40" r="10" fill="blue" />
            <line
              x1="20"
              y1="20"
              x2="90"
              y2="40"
              stroke="violet"
              stroke-width="3"
            />
          </svg>
          <div class="c21">
            <h2>009 vitae</h2>
            <p>Similique omnis</p>
          </div>
          <div class="c22">
            <h2>88</h2>
            <p>cupiditate nulla</p>
          </div>
        </div>
        <div class="container3">
          <div class="">
            <h4>👍</h4>
            <p class="big">tempore architecto</p>
            <p>nihil, quae illum qui animi maxime</p>
          </div>
          <div class="a">
            <h4>❤️</h4>
            <p class="big">dolorum obcaecati</p>
            <p>minus quasi aspernatur laboriosam tenetur! Deserunt, odio?</p>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.big-card {
  position: relative;
}
.small-card {
  position: absolute;
  top: 90px;
  right: 150px;
}
.container {
  margin-top: 20px;
  display: flex;
  flex-direction: row;
}
img {
  height: 270px;
  width: 220px;
  border-radius: 50% 0 0 50%;
}
.half-cir {
  width: 340px;
  height: 270px;
  background: rgb(250, 206, 61);
  border-radius: 50% 0 0 50%;
  display: flex;
  align-items: center;
}
h3 {
  color: #000;
  padding-left: 20px;
  font-size: 0.8rem;
}
.content1 {
  margin: 0px 10px 10px 90px;
}
p {
  font-size: 1.2rem;
  width: 180px;
}
span {
  font-weight: bold;
}
.content2 {
  margin-left: 30px;
  display: flex;
  flex-direction: row;
  column-gap: 50px;
}
.c21 {
  display: flex;
  flex-direction: column;
}
.c22 {
  display: flex;
  flex-direction: column;
}
h2 {
  margin-bottom: -2px;
}
svg {
  color: #0652dd;
}
.container2 {
  margin-top: 20px;
  display: flex;
  flex-direction: column;
}
h4 {
  font-size: 2rem;
}
.container3 {
  margin-left: 30px;
  display: flex;
  flex-direction: row;
  column-gap: 50px;
}
.big {
  font-size: 1.4rem;
}
</style>
