<template>
  <button class="container__burger">
    <div></div>
    <div></div>
    <div></div>
  </button>
</template>

<script>
export default {
  name: 'Burger',
  props: {
    open: Boolean,
  },
}
</script>

<style lang="scss" scoped>
.container__burger{
  position: absolute;
  /* top: 2%; */
  /* right: 2rem; */
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  width: 2rem;
  height: 2rem;
  background: transparent;
  border: none;
  cursor: pointer;
  padding: 0;
  z-index: 10;
  display: none;

  @media (max-width: 868px) {
    display: flex;
  }

  &:focus {
    outline: none;
  }

  div {
    width: 2rem;
    height: 0.25rem;
    background:green;
    border-radius: 10px;
    transition: all 0.3s linear;
    position: relative;
    transform-origin: 1px;
}
</style>
