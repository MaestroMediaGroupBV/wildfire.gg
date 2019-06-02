<template>
  <div class="home">
    <Header/>
    <heroSlider/>
    <StoreBanner/>
    <StoreProducts/>
    <ResultsSlider/>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";
import HeroSlider from "@/components/HeroSlider.vue";
import StoreBanner from "@/components/StoreBanner.vue";
import StoreProducts from "@/components/StoreProducts.vue";
import ResultsSlider from "@/components/ResultsSlider.vue";

export default {
  name: "home",
  components: {
    Header,
    HeroSlider,
    StoreBanner,
    StoreProducts,
    ResultsSlider,
    Footer
  }
};
</script>

<style lang="scss" scoped>
</style>
