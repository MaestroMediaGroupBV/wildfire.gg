<template>
  <div>
    <div class="grid">
      <carousel
        :per-page="1"
        :navigate-to="someLocalProperty"
        :mouse-drag="false"
        pagination-active-color="#ff7200"
        pagination-color="#555555"
        paginationSize="15"
        paginationPosition="bottom-overlay"
      >
        <slide class="slide">test</slide>
        <slide class="slide2">Slide 2 Content</slide>
      </carousel>
      <div class="containerInfo">
        <h1 class="title">TEAMS</h1>
        <h2 class="subTitle">RESULTS & EVENTS</h2>
        <p>Wildfire competes in multiple online and offline tournaments like the Copenhagen Games and the Svenska Eliteserien. Playing in studios and at big international venues. We plan to attend many events throughout Sweden & Europe in 2019. Check our most recent results and the events we plan to go to below.</p>
        <button>MORE INFO</button>
      </div>
    </div>
  </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";
export default {
  name: "ResultsSlider",

  components: {
    Carousel,
    Slide
  }
};
</script>

<style lang="scss" scoped>
.grid {
  padding-left: 140px;
  padding-right: 140px;
  display: grid;
  grid-template-columns: 1fr 1fr;
}
carousel {
  height: 600px;
}

.slide {
  background-image: url("../assets/images/teamslider.png");
  height: 400px;
}

.containerInfo {
  text-align: left;
  padding-left: 90px;
  max-width: 700px;
}
.title {
  @include resultsHeading;
}

.subTitle {
  @include resultsSubHeading;
}

p {
  @include smallText;
}

button {
  @include orangeButton;

  height: 40px;
  border-top: 0px;
  border-right: 0px;
  border-left: 0px;
  border-bottom: solid $orange-title 4px;
  border-radius: 0px;
  cursor: pointer;
  outline: none;
  text-align: left;
  padding: 0px;
  background-color: Transparent;
}
</style>