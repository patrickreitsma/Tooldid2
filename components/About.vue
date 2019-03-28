<template>
  <div class="about">
    <div class="over">
      <div class="txt">
        <h2> About me</h2>
        <div class="stripe"></div>
        <p class="info-me">
          I am Patrick, a 22 year old, self tought designer and front-end developer living in Groningen. I love listening to Hiphop and traveling. My favorite city is New York, although long flights make me kind of nervous.
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
  .about {
    width: 100%;
    height: 20%;
    color: #0d1319;
  }
  .info-me {
    text-align: center;
    padding-top: 2rem;
  }
  .over {
    position: relative;
    height: 330px;
    width: 100%;
  }
  .over:after {
    position: absolute;
    top: 0;
    left: 0;
    content: " ";
    background: url(/pic/newyork2.jpg);
    background-size: cover;
    background-position: bottom;
    width: 100%;
    height: 100%;
    opacity: 0.3;
  }
  .txt {
    text-align: center;
  }
  h2 {
    padding-left: 1rem;
    padding-top: 1rem;
  }
  .stripe {
    @include stripe;
  }
  @include breakpoint(md) {
    .info-me{
    padding: 3% 2% 0 2%;
  }
}
  </style>
