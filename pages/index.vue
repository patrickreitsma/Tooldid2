<template>
  <div>
    <index-Header />
    <index-About />
    <div class="cards">
      <index-Skills />
      <index-Stuff></index-Stuff>
    </div>
    <index-Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import About from '@/components/About.vue'
import Skills from '@/components/Skills.vue'
import Stuff from '@/components/Stuff.vue'
import Footer from '@/components/Footer.vue'

export default {
  components: {
    'index-Header': Header,
    'index-About': About,
    'index-Skills': Skills,
    'index-Stuff': Stuff,
    'index-Footer': Footer
  },
  data() {
    return {
    }
  }
}
</script>
<style scoped lang="scss">
  @include breakpoint(l) {
    .cards {
      display: flex;
      width: 100%;
    }
  }
</style>
