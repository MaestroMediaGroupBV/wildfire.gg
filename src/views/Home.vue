<template>
  <div class="home">
    <Header/>
    <heroSlider/>
    <p>this is a test</p>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";
import HeroSlider from "@/components/HeroSlider.vue";

export default {
  name: "home",
  components: {
    Header,
    HeroSlider,
    Footer
  }
};
</script>

<style lang="scss" scoped>
</style>
