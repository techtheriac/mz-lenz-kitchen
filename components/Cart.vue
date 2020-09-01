<template>
  <div class="container__cart">
    <div class="info__cart">
      <span>3 items</span>
      <span>N 500</span>
      <span>Cart</span>
    </div>
    <div class="container__button">
      <button>checkout</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Cart',
}
</script>

<style lang="scss" scoped>
.container__cart {
  max-width: 300px;
}
.info__cart {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}
</style>
