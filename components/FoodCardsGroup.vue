<template>
  <div>
    <v-card flat>
      <v-container>
        <v-row class="my-4">
          <v-card flat>
            <v-card-text>
              <v-row>
                <v-col>
                  <v-btn large depressed rounded color="#f3f6f8">Soup</v-btn>
                </v-col>

                <v-col>
                  <v-btn large depressed>Jollof Rice</v-btn>
                </v-col>

                <v-col>
                  <v-btn large depressed>Pepper Soup</v-btn>
                </v-col>
              </v-row>
            </v-card-text>
          </v-card>
        </v-row>

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
export default {
  components: {
    FoodCards,
  },
}
</script>

<style lang="scss" scoped></style>
