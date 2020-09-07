<template>
  <div class="card card-wide">
    <div class="description-container">
      <b>7 Grade Eforiro</b>
      <p>This is just a minor accumulation of text</p>
    </div>
    <img
      src="~/assets/images/Image-7.png"
      alt="pasta"
      width="186px"
      height="177px"
    />
    <div class="price-container">
      <b class="price">NGN 500 <span>per pack</span></b>
      <button>Add to Cart</button>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.card {
  background-color: var(--card-lemon);
  display: flex;
  flex-direction: column;
  padding: 1em;
  /* max-width: 400px; */

  > * + * {
    margin-top: 1em;
  }

  p {
    color: #707070d9;
  }
}

.card > img {
  align-self: center;
}

.card button {
  background-color: var(--primary-green);
  padding: 7px 18px;
  color: white;
  border-radius: 20px;
  font-size: 15px;
  outline: none;
}

.price-container {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}
</style>
