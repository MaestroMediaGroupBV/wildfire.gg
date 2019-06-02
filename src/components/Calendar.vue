<template>
  <div>
    <div class="container">
      <div class="grid">
        <p>test</p>
        <p>test</p>
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
  padding-left: 150px;
  padding-right: 150px;
}
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
</style>