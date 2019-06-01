<template>
  <div>
    <div class="header">
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
        <li>
          <router-link to="/about">
            <button>Contact</button>
          </router-link>
        </li>
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
  padding-left: 150px;
  padding-right: 150px;
  padding-top: 30px;
  padding-bottom: 30px;

  img {
    margin-bottom: -50px;
  }
}
.nav {
  text-align: right;
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
}

button {
  @include headerLink;
  width: 137px;
  height: 54px;
  border: solid $orange 1px;
  border-radius: 4px;
  background-color: $black;
  color: $orange;
}
</style>