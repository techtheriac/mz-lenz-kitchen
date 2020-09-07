<template>
  <div class="container__search">
    <input type="text" placeholder="What do you want? " />
    <IconBase class="search-icon" width="20" height="20">
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
  border-radius: 20px;
  padding: 2px 10px 2px 45px;
  display: flex;
  box-shadow: 5px 2px 15px #00000041;
  input {
    background-color: inherit;
    border: none;
    color: black;
    outline: none;
    margin-left: 5px;
    margin-right: 45px;
    font-size: 12px;

    &:focus {
      box-shadow: none;
    }
  }
}

.search-icon {
  margin-top: 9px;
}
</style>
