<template>
  <div>
    <div class="footer">
      <div class="containerFooter">
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
  height: 100%;
  margin-bottom: -20px;
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

.footerRight {
  text-align: right;
}
.containerFooter {
  padding-left: 150px;
  padding-right: 150px;
  padding-top: 50px;
}
</style>