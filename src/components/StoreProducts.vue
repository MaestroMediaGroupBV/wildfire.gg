<template>
  <div>
    <div class="container">
      <div class="grid">
        <div class="product">
          <img src="../assets/images/products/wildfire-gaming-pro-jacket.png">
          <p>WILDFIRE GAMING PRO JACKET</p>
          <p>$49.99</p>
        </div>
        <div class="product">
          <img src="../assets/images/products/wildfire-gaming-pro-hoodie.png">
          <p>WILDFIRE GAMING PRO JACKET</p>
          <p>$49.99</p>
        </div>
        <div class="product">
          <img src="../assets/images/products/wildfire-gaming-snapback.png">
          <p>WILDFIRE GAMING PRO JACKET</p>
          <p>$49.99</p>
        </div>
        <div class="product">
          <img src="../assets/images/products/wildfire-gaming-shorts.png">
          <p>WILDFIRE GAMING PRO JACKET</p>
          <p>$49.99</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "StoreProducts"
};
</script>

<style lang="scss" scoped>
.container {
  padding-left: 150px;
  padding-right: 150px;
  padding-bottom: 140px;
}

.grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
}

.product {
  img {
    height: 300px;
  }

  p {
    @include productTitle;
  }
  p:nth-child(3) {
    @include productPrice;
  }
}
</style>