<template>
  <div>
    <Header/>

    <HeroTeam/>

    <div class="container">
      <Players/>
    </div>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import HeroTeam from "@/components/headers/HeroTeam.vue";
import Players from "@/components/teams/Players.vue";
export default {
  name: "Teams",
  components: {
    Header,
    HeroTeam,
    Players,
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
.csgo {
  color: black;
}
</style>