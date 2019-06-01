

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
          <h1 class="hero-title">GOING TO <a style="color: #ff5800 ">ELITESERRIEN</a> IN STOCKHOLM!</h1>
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
  padding-left: 200px;
  padding-top: 300px;
}
.hero-title {
  @include heroTitle;
  max-width: 1200px;
}

button {
  @include heroButton;
  
  height: 40px;
  border-top: 0px;
  border-right: 0px;
  border-left: 0px;
  border-bottom: solid $white 1px;
  border-radius: 0px;
  cursor:pointer;
  outline:none;
  text-align: left;
  background-color: Transparent;
}
</style>