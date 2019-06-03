<template>
  <div>
    <div class="container">
      <div class="grid">
        <div class="left">
          <img src="../assets/images/about.png">
        </div>
        <div class="right">
          <h1>ABOUT US</h1>
          <h2>GET IN THE GAME</h2>
          <p>Established in 2018, Wildfire is one of Sweden's premier esports organizations. Over the past year, Wildfire has participated in multiple big championships in games. In 2019, founders Roland Bjorndahl and Alex Koval rebirthed the organisation under new management.Together with this new management Wildfire's player -first mentality, passion, professionalism, and innovation have led them to be recognized as a global leader in modern esports.</p>
          <button>MORE INFO</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About"
};
</script>

<style lang="scss" scoped>
.container {
  padding-left: 200px;

  padding-top: 200px;
  max-height: 400px;
}
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.left {
  text-align: left;
}

.right {
  text-align: left;
  max-width: 680px;
  h1 {
    @include resultsHeading;
    margin-top: -10px;
  }

  h2 {
    @include resultsSubHeading;
    margin-top: -20px;
  }

  p {
    @include smallText;
    margin-top: 50px;
  }
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