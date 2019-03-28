<template>
  <div class="skilss">
    <div class="content">
      <h2 class="title">Stuff</h2>
      <div class="stripe"></div>
      <div class="columns">
        <ul>
          <li>Apple</li>
          <li class="bad">Xbox</li>
          <li>Pizza</li>
          <li class="bad">Wine</li>
        </ul>
        <ul>
          <li class="bad">Android</li>
          <li>Playstation</li>
          <li class="bad">Hamburger</li>
          <li>Beer</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
  .content {
    background-color: rgba(59, 89, 152, 0.79);
    width: 100%;
    height: 350px;
    color: #ffffff;
  }
  .title{
    padding-top: 1rem;
  }
  .columns {
    padding-top: 1rem;
    height: 300px;
    display: flex;
    width: 100%;
    line-height: 3;
    font-weight: 100;
    font-size: 1.2rem;
  }
  ul {
    width: 50%;
    text-align: center;
  }
  .bad {
    color: #a2332f;
  }
  .stripe {
    @include stripe;
    border-color: #a2332f;
    background-color: #a2332f;
  }
  @include breakpoint(md) {
  }
  @include breakpoint(l) {
    .stripe{
      float: right;
    }
  .skilss{
    width: 50%;
    }
  }
</style>
