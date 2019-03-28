<template>
  <div>
    <div class="footer">
      <h3 class="copy">Copyright By Patrick Reitsma</h3>
      <p class="contact">Contact me by follow me on one of these websites.</p>
      <div class="buttons">
        <button><a href="/pic/Verantwoordingv1.pdf" download>Verantwoording </a></button>
        <button><a href="https://www.facebook.com/patrickreitsma11">Facebook </a></button>
        <button><a href="https://open.spotify.com/user/patrick_reitsma?si=Gl8wjSScQpGkyP0VMZDIDQ">Spotify</a></button>
        <button><a href="https://www.instagram.com/patrick_reitsma">Instagram</a></button>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
  div {
    width: 100%;
  }
  .footer {
    width: 100%;
    background-color: #0d1319;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  h3,
  p {
    color: #ffffff;
  }
  p {
    font-size: 0.8rem;
  }
  .buttons,
  .contact {
    display: none;
  }
  @include breakpoint(md){
    .contact {
      display: flex;
      width: 80%;
      padding-left: 5%;
    }
    .buttons{
      width: 100%;
      display: flex;
      height: 100%;
      flex-direction: column;
      align-items: flex-end;
    }
    button {
      width: 40%;
      height: 100%;
      background-color: #35404c;
      color: white;
    }
    .copy {
      display: none;
    }
  }
</style>
