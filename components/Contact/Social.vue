<template>
  <div class="social">
    <p>Volg me voor meer op mijn Social Media!</p>
    <div class="circle">
      <a href="https://www.instagram.com/patrick_reitsma"> <img src="../../static/pic/instagram1.png"/></a>
      <a href="https://www.facebook.com/patrickreitsma11"> <img src="../../static/pic/facebook1.png"/></a>
      <a href="https://open.spotify.com/user/patrick_reitsma?si=Gl8wjSScQpGkyP0VMZDIDQ"><img src="../../static/pic/spotify.png"/></a>
  </div>
  </div>
</template>

<style scoped lang="scss">
  .social {
    padding-top: 1rem;
    p{
      text-align: center;
      padding-bottom: 1rem;
    }
  }
  .circle {
    display: flex;
    flex-direction: column;
    width: 100%;
    align-items: center;
     }
  img {
    width: 150px;
    height: 150px;
    margin-bottom: 2rem;
  }
  @include breakpoint(l) {
    .circle {
      flex-direction: row;
      align-items: center;
      height: 500px;
      justify-content: space-around;
    }
  }
  @include breakpoint(xl) {
    .circle {
      height: 572px;
    }
  }
</style>
