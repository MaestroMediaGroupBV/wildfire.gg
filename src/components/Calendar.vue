<template>
  <div>
    <div class="container">
      <div class="grid">
        <div class="recentResults">
          <h1>RECENT RESULTS</h1>
          <div class="border">
            <div class="result">
              <h2>Lorem Ipsum VS Lorem Ipsum</h2>
              <div class="resultGrid">
                <div class="left">
                  <p>19-06-19</p>
                  <p>Event</p>
                </div>
                <div class="right">
                  <p>Score</p>
                </div>
              </div>
            </div>
            <div class="result">
              <h2>Lorem Ipsum VS Lorem Ipsum</h2>
              <div class="resultGrid">
                <div class="left">
                  <p>19-06-19</p>
                  <p>Event</p>
                </div>
                <div class="right">
                  <p>Score</p>
                </div>
              </div>
            </div>
            <div class="result">
              <h2>Lorem Ipsum VS Lorem Ipsum</h2>
              <div class="resultGrid">
                <div class="left">
                  <p>19-06-19</p>
                  <p>Event</p>
                </div>
                <div class="right">
                  <p>Score</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="upcomingEvents">
          <h1>UPCOMING EVENTS</h1>
          <h2>Lorem Ipsum VS Lorem Ipsum</h2>
          <p>Date</p>
          <p>Event</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Calendar"
};
</script>

<style lang="scss" scoped>
.container {
  padding-top: 100px;
  padding-left: 200px;
  padding-right: 200px;
}
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.recentResults {
  h1 {
    @include calenderHeader;
    text-align: left;
    padding-bottom: 70px;
  }
  h2 {
    @include resultTitle;
    text-align: left;
  }
  .border {
    border-right: solid $orange-title 2px;
  }
  p {
    @include resultText;
    display: inline-block;
  }
}
.upcomingEvents {
  padding-left: 90px;
  h1 {
    @include calenderHeader;
    text-align: left;
    padding-bottom: 70px;
  }
  .border {
    border-left: solid $orange-title 2px;
  }
  h2 {
    @include resultTitle;
    text-align: left;
  }
}
.result {
  padding-bottom: 60px;
}
.resultGrid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.left {
  text-align: left;
  p {
    padding-right: 50px;
  }
}

.right {
  text-align: right;
  p {
    padding-right: 65px;
  }
}
</style>