<template>
  <div id="hip">
    <nava></nava>
    <mid></mid>
  </div>
</template>

<script>
import nava from "@/components/Head/Nav.vue"
import mid from "@/components/Head/Midhead.vue"
export default {
  name: "Page-head",
  components: { nava, mid }
};
</script>

<style scoped>
#hip {
  background-image: url("@/assets/Bg-hero.svg");
  background-repeat: no-repeat;
  background-size: cover;
}

@media screen and (max-width: 375px) {
  #hip {
    height: 812px;

  }
}
</style>
