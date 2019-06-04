<template>
  <div>
    <div class="store-banner">
      <div class="store-container">
        <div class="grid">
          <div class="left">
            <div class="store-title">MERCHANDISING</div>
            <div class="store-sub-title">OFFICAL GEAR</div>
            <div class="store-small-text">Represent Wildfire like never before with your own shirt!</div>
          </div>
          <div class="right">
            <button>SHOP NOW</button>
          </div>
        </div>
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
  padding-left: 200px;
  padding-right: 200px;
}

.store-title {
  @include storeTitle;
  padding-left: 70px;
  text-align: left;
}

.store-sub-title {
  @include storeSubTitle;
  margin-top: -45px;
  text-align: left;
}

.store-small-text {
  @include storeSmallText;
  padding-top: 130px;
  text-align: left;
}

.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.right {
  padding-top: 220px;
  text-align: right;
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
  text-align: right;
  background-color: Transparent;
}
</style>