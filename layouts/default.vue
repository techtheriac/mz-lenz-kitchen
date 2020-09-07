/* eslint-disable no-console */
<template>
  <div>
    <NavBar />
    <Header />
    <nuxt />
    <Pagination />
    <Footer />
  </div>
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
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@400;700;900&display=swap');
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
body {
  font-family: Lato;
}
.toggleCart {
  display: none;
}
</style>
