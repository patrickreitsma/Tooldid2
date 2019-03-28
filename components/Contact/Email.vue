<template>
  <div class="social">
    <button><a class="email" href="mailto:preitsma@test.nl">Press me for email me!</a></button>
    <a>Or email me manually at:</a>
    <a>Preitsma@test.nl</a>
  </div>
</template>

<style scoped lang="scss">
  .social {
    background-color: #ffffff;
    color: #262f3a;
    display: flex;
    flex-direction: column;
    h3 {
      align-self: center;
      font-size: 1.5rem;
      padding-top: 0.5rem;
    }
    p {
      padding-top: 1rem;
      padding-bottom: 2rem;
      align-self: center;
      font-size: 1.2rem;
    }
    .email {
      color: #ff4500;
      display: flex;
      justify-content: center;
      font-size: 1.5rem;
      padding-top: 1rem;
      padding-bottom: 1rem;
      background-color: white;
      font-weight: bolder;
    }
    a {
      display: flex;
      justify-content: center;
      padding-bottom: 1rem;
      font-weight: bold;
    }
  }
</style>
