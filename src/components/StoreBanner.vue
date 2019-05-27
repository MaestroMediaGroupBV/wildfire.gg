<template>
  <div>
    <div class="store-banner">
      <div class="store-container">
        <div class="store-title">MERCHANDISING</div>
        <div class="store-sub-title">OFFICAL GEAR</div>
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
  padding-top: 120px;
  padding-left: 150px;
  text-align: left;
}

.store-title {
  @include storeTitle;
}

.store-sub-title {
  @include storeSubTitle;
}
</style>