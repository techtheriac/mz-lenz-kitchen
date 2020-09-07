<template>
  <div class="container__footer">
    <v-row>
      <v-col>
        <div>
          <img
            src="~/assets/images/logo.png"
            alt="mz-lenz-kitchen-logo"
            width="157px"
            height="87px"
          />
          <p>
            Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
            nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam
            erat, sed diam voluptua. At vero eos et accusam et justo duo.
          </p>
        </div>
      </v-col>
      <v-col>
        <div>
          <h4>Contact Details</h4>
          <p>Telephone: 0800007777</p>
          <p>Email: info@mzlenzkitchen.com.ng</p>
        </div>
      </v-col>
      <v-col>
        <div>
          <h4>Follow us</h4>
          <p>FB: mrslenzkitchen</p>
          <p>TW: @mrslenzkitchen</p>
          <p>IG @mrslenzkitchen</p>
        </div>
      </v-col>
    </v-row>
  </div>
</template>
<script>
export default {
  name: 'Footer',
}
</script>

<style lang="scss" scoped>
.container__footer {
  background-color: #707070 !important;
  color: var(--background-offwhite);
  padding: 2em;
}

@media (min-width: 35em) {
  .container__footer {
    padding: 2em 2em 2em 3.5em;
  }
}

.col {
  align-self: flex-end;
}
</style>
