<template>
  <div>
    <Header/>
    <HeroMedia/>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import HeroMedia from "@/components/headers/HeroMedia.vue";
export default {
  name: "Media",
  components: {
    Header,
    HeroMedia,
    Footer
  }
};
</script>

<style lang="scss" scoped>
</style>