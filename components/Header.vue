<template>
  <div class="landing-page">
    <div class="container__landing px-4 mb-3">
      <h1 class="heading-text">
        Bespoke Meals, <br />
        Just the way you want it
      </h1>
      <p>Imagine sampling confectioneries from around the world</p>
      <button class="btn__home">GO TO MENU</button>
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
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('../assets/images/mobile.png') center center;
  background-size: contain;
  background-repeat: no-repeat;
  color: white;
  /* display: flex; */
  /* align-items: center;
  justify-content: center; */
}

.container__landing {
  margin-top: 4em;
}

.btn__home {
  background-color: var(--primary-green);
  padding: 9px 18px;
  color: white;
  border-radius: 20px;
  font-size: 14px;
  outline: none;
  margin-top: 1.7em;
  margin-bottom: 1em;
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
    color: #000;

    h1 {
      font-size: 3rem;
    }
  }

  .btn__home {
    background-color: var(--primary-green);
    padding: 9px 18px;
    color: white;
    border-radius: 20px;
    font-size: 16px;
    outline: none;
    margin-top: 2em;
  }
}

/* .landing-page {
  background: url('../assets/images/mobile.png');
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  background-origin: content-box;
  padding: 4rem;
  text-shadow: 0.1em 0.1em 0.3em #000;
  background-color: #efecf5;
  width: 100%;

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
 */
</style>
