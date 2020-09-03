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
  color: #fff;
  box-shadow: 0px 10px 20px #00000041;
  border-radius: 0 0 20px 20px;
  position: fixed;
  top: 0;
  z-index: 9;
  right: 7em;
}
.info__cart {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
  background-color: #000;
  padding: 10px;
}

.container__button {
  color: whitesmoke;
  padding: 10px;
  border-radius: 0 0 20px 20px;
  button {
    background-color: var(--primary-green);
    padding: 8px 50px;
    border-radius: 20px;
    text-transform: uppercase;
    font-size: 0.9rem;
  }
}

@media (max-width: 35em) {
  .container__cart {
    display: none;
  }
}
</style>
