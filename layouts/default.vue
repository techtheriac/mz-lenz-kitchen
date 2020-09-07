/* eslint-disable no-console */
<template>
  <v-app>
    <NavBar />
    <Header />
    <nuxt />
    <Pagination />
    <Footer />
  </v-app>
</template>

<script>
import Footer from '~/components/Footer.vue'
import Header from '~/components/Header.vue'
import Pagination from '~/components/Pagination.vue'
export default {
  components: {
    Footer,
    Header,
    Pagination,
  },
}
</script>

<style lang="scss">
:root {
  box-sizing: border-box;
  /* font-size: calc(1vw + 0.6em); */

  --primary-green: #214b15;
  --background-offwhite: #efecf5;
  --card-lemon: #f3f6f8;
  --grey: #707070;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}
.toggleCart {
  display: none;
}
</style>
