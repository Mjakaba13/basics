<template>
  <heades></heades>
  <mid></mid>
  <belt></belt>
  <blop></blop>
  <best></best>
  <join></join>
  <foot></foot>
</template>
<!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->

<script>
import heades from "@/components/Head/Page-head.vue";
import mid from "@/components/Mid/First.vue";
import belt from "@/components/Belt/Eins.vue";
import blop from "@/components/Blow/Blop.vue";
import best from "@/components/Deal/Best.vue";
import join from "@/components/Joiner/Joint.vue";
import foot from "@/components/Footer/Foot.vue"
export default {
  name: "App",
  components: { heades, mid, belt, blop, best, join, foot },
};
</script>

<style>
#app {
  font-family: "Roboto", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@media screen and (max-width: 375px) {
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  #app {
    font-family: "Roboto", sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    /* text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
  }
}
</style>
