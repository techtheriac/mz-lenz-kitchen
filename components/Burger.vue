<template>
  <button class="container__burger" @click="toggle">
    <div></div>
    <div></div>
    <div></div>
  </button>
</template>

<script>
export default {
  name: 'Burger',
  props: {
    showNav: Boolean,
  },
  methods: {
    toggle(e) {
      this.$emit('onToggle')
    },
  },
}
</script>

<style lang="scss" scoped>
.container__burger {
  position: absolute;
  top: 2%;
  right: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  width: 2rem;
  height: 2rem;
  background: transparent;
  border: none;
  padding: 0;
  z-index: 10;

  &:focus {
    outline: none;
  }

  div {
    width: 2rem;
    height: 0.25rem;
    background: green;
    border-radius: 10px;
    transition: all 0.3s linear;
    position: relative;
    transform-origin: 1px;
  }
}

@media (min-width: 35em) {
  .container__burger {
    display: none;
  }
}
</style>
