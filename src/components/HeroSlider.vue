

<template>
  <div>
    <carousel
      :per-page="1"
      :navigate-to="someLocalProperty"
      :mouse-drag="false"
      pagination-active-color="#ff7200"
      pagination-color="#555555"
      paginationSize="15"
      paginationPosition="bottom-overlay"
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
  height: 1070px;
}

.slide2 {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-image: url("../assets/images/slider.png");
  height: 1000px;
}
.hero-container {
  max-width: 1200px;
  text-align: left;
  padding-left: 150px;
  padding-top: 50px;
}
.hero-title {
  @include heroTitle;
  max-width: 1100px;
}

.hero-sub-title {
  @include heroSubTitle;
  max-width: 1200px;
  margin-top: -60px;
  padding-bottom: 20px;
}
button {
  @include heroButton;
  width: 170px;
  height: 51px;
  border: solid $hero-btn 0px;
  border-radius: 4px;
  background-color: $hero-btn;
}
</style>