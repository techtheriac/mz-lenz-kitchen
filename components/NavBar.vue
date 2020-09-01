<template>
  <nav class="nav-bar">
    <Search />
  </nav>
</template>

<script>
import Search from './Search.vue'
export default {
  components: {
    Search,
  },
}
</script>

<style lang="scss" scoped>
.nav-bar {
  display: flex;
}
</style>
