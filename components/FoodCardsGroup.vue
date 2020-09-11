<template>
  <div>
    <v-card flat>
      <v-container>
        <Stripe />
        <v-row>
          <v-col cols="12" lg="5">
            <FoodCards />
          </v-col>
          <v-col>
            <FoodCards />
          </v-col>
          <v-col>
            <FoodCards />
          </v-col>
        </v-row>

        <v-row>
          <v-col>
            <FoodCards />
          </v-col>
          <v-col cols="12" lg="5">
            <FoodCards />
          </v-col>
          <v-col>
            <FoodCards />
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </div>
</template>

<script>
import FoodCards from '~/components/FoodCards.vue'
import Stripe from '~/components/Stripe.vue'
export default {
  components: {
    FoodCards,
    Stripe,
  },
}
</script>

<style lang="scss" scoped>
/* .stripe-group {
  background-color: white;
}
.empty_stripe {
  background-color: #c5d2da;
  margin-left: 23em;
  width: 404px;
  height: 64px;
} */

@media (max-width: 35em) {
  .empty_stripe {
    display: none;
  }
}
</style>
