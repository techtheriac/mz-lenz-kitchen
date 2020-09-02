<template>
  <nav class="nav-bar">
    <img
      src="~/assets/images/logo.png"
      alt="mz-lenz-kitchen-logo"
      class="logo"
    />

    <div class="container__group">
      <ul class="group__nav">
        <li><a href="">menu</a></li>
        <li><a href="">about us</a></li>
        <li><a href="">contact</a></li>
      </ul>

      <div class="group__search">
        <p>My Location: <b>Jerry Irabe Lekki Phase 1</b></p>
        <!-- Search component-->
        <Search />
      </div>
    </div>
    <Burger @onToggle="toggle" />
    <Menu :class="{ toggleNav: isActive }" />
    <Cart />
  </nav>
</template>

<script>
import Burger from '~/components/Burger.vue'
import Menu from '~/components/Menu.vue'
import Search from '~/components/Search.vue'
import Cart from '~/components/Cart.vue'
// import AppDrawer from '~/components/AppDrawer.vue'
export default {
  components: {
    Burger,
    Menu,
    Search,
    Cart,
    // AppDrawer,
  },
  data() {
    return {
      isActive: false,
    }
  },
  methods: {
    toggle() {
      this.isActive = !this.isActive
    },
  },
}
</script>

<style lang="scss" scoped>
.nav-bar {
  display: flex;
  background-color: #efecf5;
  flex-direction: row;
  .logo {
    width: 100px;
    height: 53px;
    align-self: flex-end;
    margin-left: 2.5em;
    margin-top: 0.7em;
  }
}
.group__search {
  display: flex;
  flex-direction: column;
  margin-left: 7em;
  justify-content: center;
  align-items: center;
  p {
    font-size: 0.8rem;
    color: var(--grey);
    margin-top: 10px;
  }
  b {
    color: black;
    font-size: 1rem;
  }
}

.group__nav {
  display: flex;
  flex-direction: row;
  list-style-type: none;
  margin-top: 2em;
  margin-left: 2em;
  > * + * {
    padding-left: 2em;
  }
  a {
    text-decoration: none;
    text-transform: uppercase;
    color: #000;
    font-size: 0.7rem;
  }
}

.toggleNav {
  transform: translateX(0);
  display: flex;
}

.container__group {
  display: flex;
  flex-direction: row;
}

@media (max-width: 35em) {
  .container__group {
    display: none;
  }
}
</style>
