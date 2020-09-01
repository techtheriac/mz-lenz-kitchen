<template>
  <nav class="nav-bar">
    <img
      src="~/assets/images/logo.png"
      alt="mz-lenz-kitchen-logo"
      width="157px"
      height="87px"
    />
    <Burger />
    <Menu />
  </nav>
</template>

<script>
import Burger from '~/components/Burger.vue'
import Menu from '~/components/Menu.vue'
export default {
  components: {
    Burger,
    Menu,
  },
}
</script>

<style lang="scss" scoped>
.nav-bar {
  display: flex;
  background-color: #efecf5;
}
</style>
