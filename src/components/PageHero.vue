<template>
  <div>
    <div class="hero">
      <div class="container">
        <div class="title">OUR TEAMS</div>
        <div class="subTitle">LINE UPS</div>
        <button>MORE INFO</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PageHero",
};
</script>

<style lang="scss" scoped>
.container {
  padding-left: 200px;
  padding-right: 200px;
}
.hero {
  background-image: url("../assets/images/team-header.png");
  height: 500px;
  margin-top: -25px;
}

.title {
  @include storeTitle;
  padding-left: 70px;
  text-align: left;
}

.subTitle {
  @include storeSubTitle;
  margin-top: -45px;
  text-align: left;
}

button {
  @include heroButton;
  margin-top: 100px;
  padding: 0px;
  height: 40px;
  border-top: 0px;
  border-right: 0px;
  border-left: 0px;
  border-bottom: solid $white 4px;
  border-radius: 0px;
  cursor: pointer;
  outline: none;

  background-color: Transparent;
}
</style>