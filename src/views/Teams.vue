<template>
  <div>
    <Header/>

    <PageHero/>
    <div class="container"></div>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import PageHero from "@/components/PageHero.vue";
export default {
  name: "Teams",
  components: {
    Header,
    PageHero,
    Footer
  }
};
</script>

<style lang="scss" scoped>
.container {
  padding-left: 200px;
  padding-right: 200px;
}

.grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
}
</style>