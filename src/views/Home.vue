<template>
  <div class="home">
    <Header/>
    <p>this is a test</p>
    <Footer/>
  </div>
</template>

<script>
// @ is an alias to /src
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";

export default {
  name: "home",
  components: {
    Header,
    Footer
  }
};
</script>

<style lang="scss" scoped>
</style>
