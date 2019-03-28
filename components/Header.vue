<template>
  <div class="header">
    <div class="title">
      <h1> Patrick Reitsma</h1>
    </div>
    <div class="sub-title">
      <h3> MAKING IDEAS HAPPEN</h3>
    </div>
    <div class="contact">
      <b-button class="contact-button">
        <nuxt-link to="Contact">Contact!</nuxt-link>
      </b-button>
    </div>
  </div>
</template>

<style scoped lang="scss">
  .header {
   background-color: #262f3a;
   height: 400px;
   width: 100%;
   display: flex;
   justify-content: center;
   align-items: center;
   flex-direction: column;
   color: #ffffff;
    margin: 0;
    padding: 0;
  }
  h1 {
   color: white;
  }
  .sub-title {
   margin-bottom: 35px;
  }
  .contact-button {
   background-color: #0d1319;
   border-color: #ffffff;
    text-decoration: none;
   }
  @include breakpoint(md) {
  }
  @include breakpoint(l) {
  }
</style>
