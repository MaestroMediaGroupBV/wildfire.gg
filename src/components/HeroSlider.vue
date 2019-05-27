

<template>
  <div>
    <carousel
      :per-page="1"
      :navigate-to="someLocalProperty"
      :mouse-drag="false"
      pagination-active-color="#ff7200"
      pagination-color="#555555"
      paginationSize="15"
      paginationPosition="bottom"
    >
      <slide class="slide">
        <div class="hero-container">
          <h1 class="hero-title">GOING TO ELITESERRIEN IN STOCKHOLM!</h1>
          <h2
            class="hero-sub-title"
          >The wildfire male team have successfully qualified to compete at the inferno online studio.</h2>
          <button>MORE INFO</button>
          <p>slide 1</p>
        </div>
      </slide>
      <slide class="slide2">Slide 2 Content</slide>
    </carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";
export default {
  name: "HeroSlider",

  components: {
    Carousel,
    Slide
  }
};
</script>

<style lang="scss" scoped>
.slide {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-image: url("../assets/images/slider.png");
  height: 1000px;
}

.slide2 {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-image: url("../assets/images/slider.png");
  height: 1000px;
}
.hero-container {
  max-width: 1000px;
  text-align: left;
  padding-left: 150px;
  padding-top: 100px;
}
.hero-title {
  @include heroTitle;
  max-width: 700px;
  margin-bottom: -10px;
}

.hero-sub-title {
  @include heroSubTitle;
  max-width: 750px;
}
button {
  @include heroButton;
  width: 170px;
  height: 51px;
  border: solid $orange 0px;
  border-radius: 4px;
  background-color: $orange;
}
</style>