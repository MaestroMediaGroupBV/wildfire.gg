<template>
  <div>
    <Header/>
    <p>this is the teams page</p>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "Teams",
  components: {
    Header,
    PageHeader,
    Footer
  }
};
</script>

<style lang="scss" scoped>
</style>