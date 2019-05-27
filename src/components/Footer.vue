<template>
  <div>
    <div class="footer">
      <div class="container">
        <div class="footerNav">
          <ul>
            <li>
              <router-link to="/">ABOUT US</router-link>
            </li>
            <li>
              <router-link to="/about">TEAMS</router-link>
            </li>
            <li>
              <router-link to="/">PARTNERS</router-link>
            </li>
            <li>
              <router-link to="/about">MEDIA</router-link>
            </li>
            <li>
              <router-link to="/">MERCHANDISING</router-link>
            </li>
          </ul>
        </div>
        <div class="footerRight">
          <p>test</p>
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
  height: 205px;
}

.footerNav {
  text-align: left;
  padding-left: 150px;
  a {
    @include footerLink;
    text-decoration: none;
    color: grey;
  }
  ul li {
    list-style: none;
  }

  ul li a:hover {
    color: white;
  }
}

.footerRight {
  text-align: right;
}
.container {
}
</style>