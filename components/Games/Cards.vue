<template>
  <div>
    <h1 class="title">Games</h1>
    <div class="stripe"></div>
    <div class="cards">
      <div class="cardd">
        <img src="../../static/pic/uc1.jpg"/>
        <h2 class="hcard">Uncharted</h2>
      </div>
      <div class="cardd">
        <img src="../../static/pic/cod1.jpg"/>
        <h2 class="hcard">Call of duty</h2>
      </div>
      <div class="cardd ">
        <img src="../../static/pic/lou1.jpg"/>
        <h2 class="hcard">Last of Us</h2>
      </div>
    </div>
    <div class="cardstwo">
      <div class="cardd">
        <img src="../../static/pic/bfhover.png"/>
        <h2 class="hcard">Battlefield V</h2>
      </div>
      <div class="cardd five">
        <img src="../../static/pic/fifa.jpg"/>
        <h2 class="hcard">Fifa</h2>
      </div>
      <div class="cardd">
        <img src="../../static/pic/fort.jpg"/>
        <h2 class="hcard">Fortnite</h2>
      </div>
    </div>
  </div>
  </div>
</template>

<style scoped lang="scss">
  .cards {
    width: 100%;
  }
  .stripe {
    @include stripe;
    border-color: #262F3A;
    background-color: #262F3A;
  }
  .title {
    padding-top: 1rem;
    padding-bottom: 1rem;
    text-shadow: 1px 1px 2px #cdcdcd;
    color: #333;
  }
  .cardd {
    background-color: #262f3a;
    margin: 5% 3% 5% 3%;
    border-radius: 15px;
    height: 400px;
    display: flex;
    justify-content: center;
    align-content: center;
  }
  .hcard {
    align-self: center;
    color: #ffffff;
    text-shadow: 2px 2px 4px #342abe;
  }
  img{
    width: 100%;
    height: auto;
    border-radius: 15px;
    opacity: 0.4;
  }
  .cardd>img {
    display: none;
  }
  .cardd:hover>img {
    display: block;
  }
  .cardd:hover>.hcard {
    display: none;
  }
  @include breakpoint(md){
    template {
      margin: 0 2% 0 2%;
    }
    .title{
      display: flex;
      justify-content: center;
      margin-left: 2%;
    }
    .stripe{
      margin-bottom: 2rem;
    }
    .cards {
      width: 96%;
      display: flex;
      margin-left: 2%;
      margin-right: 2%;
    }
    .cardd {
      height: 300px;
      width: 50%;
      margin: 0;
      border-radius: 0;
      box-shadow: none;
    }
    .cardstwo {
      display: flex;
      width: 96%;
      margin-left: 2%;
      margin-right: 2%;
      margin-bottom: 10%;
    }
    img {
      border-radius: 0;
    }
  }
  @include breakpoint(l) {
    .cardd {
      height: 400px;
    }
  }
  @include breakpoint(xl) {
    .cardd {
      height: 700px;
    }
  }
</style>
