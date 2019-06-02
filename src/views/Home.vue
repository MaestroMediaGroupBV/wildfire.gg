<template>
  <div class="home">
    <Header/>
    <heroSlider/>
    <StoreBanner/>
    <StoreProducts/>
    <ResultsSlider/>
    <Calendar/>
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
import Calendar from "@/components/Calendar.vue";
export default {
  name: "home",
  components: {
    Header,
    HeroSlider,
    StoreBanner,
    StoreProducts,
    ResultsSlider,
    Calendar,
    Footer
  }
};
</script>

<style lang="scss" scoped>
</style>
