<template>
  <div>
    <div class="container">
      <div class="grid">
        <div class="containerHeader">
          <h2>Gentlemans</h2>
          <h2>Ladies</h2>
          <hr />
        </div>
        <div class="player">
          <div class="name">Jordan Gill</div>
          <div class="sub">Team Captain</div>
          <div class="socials"></div>
        </div>
        <div class="player">
          <div class="name">Jordan Gill</div>
          <div class="sub">Team Captain</div>
          <div class="socials"></div>
        </div>
        <div class="player">
          <div class="name">Jordan Gill</div>
          <div class="sub">Team Captain</div>
          <div class="socials"></div>
        </div>
        <div class="player">
          <div class="name">Jordan Gill</div>
          <div class="sub">Team Captain</div>
          <div class="socials"></div>
        </div>
        <div class="player">
          <div class="name">Jordan Gill</div>
          <div class="sub">Team Captain</div>
          <div class="socials"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Players"
};
</script>

<style lang="scss" scoped>
.container {
}
.grid {
  display: grid;
  grid-template-rows: 1fr 1fr;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
}

.containerHeader {
  h2 {
  }
}
.player {
  background-color: pink;
  border: 5px solid cyan;
  height: 250px;
  width: 250px;
}
</style>