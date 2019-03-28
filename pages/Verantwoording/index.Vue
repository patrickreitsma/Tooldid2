<template>
  <div class="verantwoordingpage">
    <div class="title">
      <h1>Verantwoording</h1>
      <div class="stripe"></div>
    </div>
    <index-Footer />
  </div>
</template>

<style scoped lang="scss">
  .verantwoordingpage {
    background-color: #262F3A;
    height: 100%;
  }
  .title {
    @include title;
    color: white;
    width: 100%;
  }
  .stripe {
    @include stripe;
    margin-bottom: 1rem;
    background-color: #ffffff;
  }
</style>
