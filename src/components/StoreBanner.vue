<template>
  <div>
    <div class="store-banner">
      <div class="store-container">
        <div class="store-title">MERCHANDISING</div>
        <div class="store-sub-title">OFFICAL GEAR</div>
        <div class="store-small-text">Represent Wildfire like never before with your own shirt!</div>
        <button>SHOP NOW</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "StoreBanner"
};
</script>

<style lang="scss" scoped>
.store-banner {
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  background-image: url("../assets/images/store-banner.png");
  height: 600px;
}

.store-container {
  padding-top: 130px;
  padding-left: 150px;
  text-align: left;
}

.store-title {
  @include storeTitle;
  padding-left: 70px;
}

.store-sub-title {
  @include storeSubTitle;
  margin-top: -45px;
}

.store-small-text {
  @include storeSmallText;
  padding-top: 130px;
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