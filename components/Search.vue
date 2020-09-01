<template>
  <div class="container__search">
    <input type="text" placeholder="What do you want?" />
    <IconBase class="search-icon">
      <SearchIcon />
    </IconBase>
  </div>
</template>

<script>
import SearchIcon from './legos/SearchIcon.vue'
import IconBase from './legos/IconBase.vue'
export default {
  components: {
    SearchIcon,
    IconBase,
  },
}
</script>

<style lang="scss" scoped>
.container__search {
  background-color: var(--background-offwhite);
  border-radius: 10px;
  padding: 0.5rem;
  display: flex;

  input {
    background-color: inherit;
    border: none;
    color: black;
    outline: none;
    padding-right: 5px;

    &:focus {
      box-shadow: none;
    }
  }
}

.search-icon {
  margin-top: 9px;
}
</style>
