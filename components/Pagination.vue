<template>
  <div class="text-center">
    <v-pagination v-model="page" :length="9" :total-visible="5"></v-pagination>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
.text-center .v-pagination__item,
.v-pagination__navigation {
  box-shadow: none !important;
}
</style>
