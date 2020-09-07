<template>
  <div class="stripe">
    <v-row>
      <v-col>
        <v-btn large depressed rounded color="#c5d2da">Soup</v-btn>
      </v-col>

      <v-col>
        <v-btn large depressed>Jollof Rice</v-btn>
      </v-col>

      <v-col>
        <v-btn large depressed>Pepper Soup</v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'Stripe',
}
</script>

<style lang="scss" scoped>
.stripe {
  background-color: #c5d2da;
}
.row {
  background-color: var(--card-lemon);
  width: 75%;
}
.row:nth-child(3) {
  margin-right: 3rem;
}
</style>
