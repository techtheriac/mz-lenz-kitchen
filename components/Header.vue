<template>
  <div class="landing-page">
    <div class="container__landing">
      <h1 class="heading-text">
        Bespoke Meals, <br />
        Just the way you want it
      </h1>
      <p>Imagine sampling confectioneries from around the world</p>
      <button>GO TO MENU</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style lang="scss" scoped>
.landing-page {
  background: url('../assets/images/mobile.png');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  background-origin: content-box;
  padding: 4rem;
  text-shadow: 0.1em 0.1em 0.3em #000;
  background-color: #efecf5;

  @media (max-width: 375px) {
    background-size: 158% 74%;
  }

  p {
    margin-top: 1rem;
  }
  button {
    background-color: var(--primary-green);
    padding: 9px 18px;
    color: white;
    border-radius: 20px;
    font-size: 16px;
    outline: none;
    margin-top: 3em;
  }
}

@media (min-width: 35em) {
  .landing-page {
    background: url('../assets/images/landing.png');
    background-position: bottom right;
    background-size: 65% 83%;
    text-shadow: none;
    padding: 7rem 7rem 15rem 3.5rem;
    background-color: #efecf5;
    background-repeat: no-repeat;

    P {
      color: #707070;
    }

    h1 {
      font-size: 3rem;
    }
  }
  .container-landing {
    margin-top: 5rem;
    margin-bottom: 5rem;
  }
}
</style>
