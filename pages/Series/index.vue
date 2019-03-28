<template>
  <div class="seriespage">
    <div class="title">
      <h1>Series</h1>
      <div class="stripe"></div>
    </div>
    <Series-Cards v-for="(card, index) in cards" :value="card" :key="index"/>
    <index-Footer />
  </div>
</template>

<script>
import Cards from '@/components/Series/Cards.vue'
import Footer from '@/components/Footer.vue'

export default {
  components: {
    'Series-Cards': Cards,
    'index-Footer': Footer
  },
  data() {
    return {
      cards: [
        {
          img: '/pic/twd.jpg',
          title: 'The Walking Dead'
        }, {
          img: '/pic/puni.jpg',
          title: 'The Punisher'

        }, {
          img: '/pic/orange1.jpg',
          title: 'Orange Is The New Black'
        }, {
          img: '/pic/prison1.jpg',
          title: 'Prison Break'
        }
      ]
    }
  }
}
</script>
<style scoped lang="scss">
  .seriespage{
    background-color:  #262F3A;
    height: 100%;
    display: flex;
    flex-wrap: wrap;
    width: 100%;
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
  @include breakpoint(l) {
  }

</style>
