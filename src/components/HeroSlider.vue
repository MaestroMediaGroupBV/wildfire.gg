

<template>
  <div>
    <carousel
      :per-page="1"
      :navigate-to="someLocalProperty"
      :mouse-drag="true"
      pagination-active-color="#ff7200"
      pagination-color="#555555"
      paginationSize="15"
    >
      <slide class="slide" id="slide-image">
        <div class="hero-container">
          <h1 class="hero-title">
            GOING TO
            <a style="color: #ff5800 ">ELITESERRIEN</a> IN STOCKHOLM!
          </h1>
          <button>MORE INFO</button>
        </div>
      </slide>
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
  max-height: 1100px;
}
.VueCarousel-pagination {
  .VueCarousel-pagination--bottom-overlay {
    bottom: 400px;
  }
}
.VueCarousel-dot-container {
}

#slide-image {
  background-image: url("../assets/images/slider.png");
  height: 100%;
  padding-bottom: 500px;
  margin-top: -10px;
  margin-bottom: -300px;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
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
  padding: 0px;
  height: 40px;
  border-top: 0px;
  border-right: 0px;
  border-left: 0px;
  border-bottom: solid $white 4px;
  border-radius: 0px;
  cursor: pointer;
  outline: none;
  text-align: left;
  background-color: Transparent;
}
</style>