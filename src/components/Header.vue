<template>
  <div>
    <div class="header">
      <div class="grid">
        <div class="logo">
          <img src="../assets/logo.png">
        </div>
        <div class="nav">
          <li>
            <router-link to="/">ABOUT US</router-link>
          </li>
          <li>
            <router-link to="/about">TEAMS</router-link>
          </li>
          <li>
            <router-link to="/about">PARTNERS</router-link>
          </li>
          <li>
            <router-link to="/about">MEDIA</router-link>
          </li>
          <li>
            <router-link to="/about">MERCHANDISING</router-link>
          </li>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>

<style lang="scss" scoped>
.header {
  background-color: black;
  padding-left: 200px;
  padding-right: 200px;
  padding-top: 30px;
  padding-bottom: 30px;
}
.nav {
  text-align: right;
  padding-top: 30px;
  padding-bottom: 30px;
  a {
    @include headerLink;
    text-decoration: none;

    &.router-link-exact-active {
      color: white;
    }
  }

  li {
    display: inline;
    padding-right: 40px;
  }
}

.logo {
  text-align: left;
  width: 100%;
  height: 100%;
  padding-top: 10px;
}
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
</style>