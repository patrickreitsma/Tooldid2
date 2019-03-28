<template>
  <div>
    <div class="content">
      <div class="cards">
        <img :src="value.img"/>
      </div>
      <div class="txt">
        <h2>{{ value.title }}</h2>
      </div>
      <div class="stripe"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'card',
  props: {
    value: {
      required: true
    }
  }
}
</script>

<style scoped lang="scss">
  .content,
  div
  {
    width: 96%;
    margin-bottom: 1%;
  }
  .txt {
    display: flex;
    justify-content: center;
    margin-left: 1.2rem;
  }
  .stripe {
    @include stripe;
    margin-bottom: 1rem;
    background-color: #ffffff;
    color: white;
    margin-left: 6%;
  }
  img {
    width: 100%;
    height: 100%;
  }
  .cards {
    border: 1px solid #ffffff;
    height: 402px;
    margin: 0 6% 0 6%;
  }
  .txt {
    h2{
      color: #ffffff;
      font-size: 1.8rem;
      font-weight: 100;
    }
    .stripe {
    margin-left: 6%;
    color: #ffffff;
    background-color: #ffffff;
    }
  }
  @include breakpoint(md){
    .content{
      height: 100%;
      width: 100%;
      display: flex;
      flex-wrap: wrap;
      align-content: baseline;
    }
    .cards,
    .txt {
      width: 40%;
    }
    .txt {
      align-self: center;
    }
    .stripe {
      display: none;
    }
  }
  @include breakpoint(l) {
    div,
    .content{
      width: 50%;
      display: flex;
      justify-content: center;
      margin-bottom: 2%;
    }
    .cards,
    .txt{
      width: 100%;
    }
    .cards {
      height: 370px;
    }
  }
  @include breakpoint(xl) {
    .cards {
      height: 405px;
    }
  }
</style>
