<template>
  <div class="skilss">
    <div class="content">
      <h2 class="title">Skills</h2>
      <div class="stripe"></div>
      <div class="columns">
        <ul>
          <li>Invision</li>
          <li>Photoshop</li>
          <li>Indesign </li>
          <li>Illustrator</li>
        </ul>
        <ul>
          <li>HTML5</li>
          <li>CSSS3</li>
          <li>SCSS</li>
          <li>Vue.js</li>
        </ul>
      </div>
    </div>

  </div>
</template>

<style scoped lang="scss">
  .content {
    background-color: #f9f9f9;
    width: 100%;
    height: 350px;
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
  .stripe {
    @include stripe;
  }
  @include breakpoint(md) {
  }
  @include breakpoint(l) {
    .skilss{
    width: 50%;
    }
  }
</style>
