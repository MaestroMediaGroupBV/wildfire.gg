<template>
  <div>
    <div class="footer">
      <div class="container">
        <div class="grid">
          <div class="footerNav">
            <li>
              <router-link to="/">ABOUT US</router-link>
            </li>
            <li>
              <router-link to="/">TEAMS</router-link>
            </li>
            <li>
              <router-link to="/">PARTNERS</router-link>
            </li>
            <li>
              <router-link to="/">MEDIA</router-link>
            </li>
            <li>
              <router-link to="/">MERCHANDISING</router-link>
            </li>
          </div>
          <div class="right">
            <img src="../assets/logo-footer.png">

            <img src="../assets/images/icons/insta.png" style="padding-bottom: 15px">
            <img src="../assets/images/icons/twitter.png" style="padding-bottom: 15px">
            <img src="../assets/images/icons/facebook.png" style="padding-bottom: 15px">
            <h1>© WILDFIRE GAMING 2019 - ALL RIGHTS RESERVED</h1>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style lang="scss" scoped>
.footer {
  background-image: url("../assets/images/footer.png");
  background-repeat: no-repeat;
  height: 100%;
}

.footerNav {
  text-align: left;

  a {
    @include footerLink;
    text-decoration: none;
    color: grey;
  }
  li {
    list-style: none;
    padding-bottom: 5px;
  }

  li a:hover {
    color: white;
  }
}

.right {
  text-align: right;
  img {
    padding-left: 25px;
  }
}

.container {
  padding-left: 200px;
  padding-right: 200px;
  padding-top: 40px;
  padding-bottom: 40px;
}
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
h1 {
  @include copyright;
  padding-top: 20px;
}
</style>