<template>
  <div class="menu">
    <a href="">Menu</a>
    <a href="">About Us</a>
    <a href="">Contact</a>
    <Search />
  </div>
</template>

<script>
import Search from '~/components/Search.vue'
export default {
  name: 'Menu',
  components: {
    Search,
  },
}
</script>

<style lang="scss" scoped>
.menu {
  flex-direction: column;
  justify-content: center;
  background: #33391b;
  height: 100%;
  text-align: left;
  padding: 2rem;
  position: absolute;
  top: 0;
  right: 0;
  transition: transform 0.3s ease-in-out;
  transform: translateX(100%);
  display: none;
  z-index: 1;
  overflow: hidden;

  a {
    font-size: 2rem;
    text-transform: uppercase;
    padding: 2rem 0;
    font-weight: bold;
    letter-spacing: 0.5rem;
    color: wheat;
    text-decoration: none;
    transition: color 0.3s linear;

    /* @media (max-width: '576px') {
      font-size: 1.5rem;
      text-align: center;
    } */

    &:hover {
      color: '#343078';
    }
  }
}

@media (min-width: 35em) {
  .menu {
    display: none;
  }
}
</style>
