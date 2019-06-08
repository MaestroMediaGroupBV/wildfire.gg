<template>
  <div>
    <Header/>
    <HeroPartner/>
    <div class="container">
      <div class="grid">
        <img src="../assets/images/partners/21ilab.png" label="Partner 21ilab">
        <img src="../assets/images/partners/rogue-energy.png" label="Partner Rogue Energy">
        <img src="../assets/images/partners/21ilab.png" label="Partner 21ilab">
        <img src="../assets/images/partners/rogue-energy.png" label="Partner Rogue Energy">
        <img src="../assets/images/partners/21ilab.png" label="Partner 21ilab">
        <img src="../assets/images/partners/rogue-energy.png" label="Partner Rogue Energy">

        <img src="../assets/images/partners/21ilab.png" label="Partner 21ilab">
        <img src="../assets/images/partners/rogue-energy.png" label="Partner Rogue Energy">
        <img src="../assets/images/partners/21ilab.png" label="Partner 21ilab">
        <img src="../assets/images/partners/rogue-energy.png" label="Partner Rogue Energy">
        <img src="../assets/images/partners/21ilab.png" label="Partner 21ilab">
        <img src="../assets/images/partners/rogue-energy.png" label="Partner Rogue Energy">
      </div>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import HeroPartner from "@/components/headers/HeroPartner.vue";
export default {
  name: "Partners",
  components: {
    Header,
    HeroPartner,
    Footer
  }
};
</script>

<style lang="scss" scoped>
.container {
  margin-left: 200px;
  margin-right: 200px;
  padding-bottom: 120px;
}
.grid {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  grid-template-rows: 2;
  grid-column-gap: 50px;
  overflow: hidden;
  img {
    padding-top: 120px;
  }
}
</style>