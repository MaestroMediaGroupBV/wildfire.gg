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
  background-color: black;

  width: 100%;
  height: 300px;
}

.footerNav {
  padding-top: 50px;
  text-align: left;
  a {
    @include footerLink;
    text-decoration: none;
    color: grey;
  }
  ul li {
    list-style: none;
    padding-bottom: 15px;
  }

  ul li a:hover {
    color: white;
  }
}

.container {
  padding-left: 150px;
}
</style>