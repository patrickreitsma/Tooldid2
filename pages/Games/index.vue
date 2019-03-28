<template>
  <div>
    <Games-Cards />
    <index-Footer />
  </div>
</template>

<script>
import Cards from '@/components/Games/Cards.vue'
import Footer from '@/components/Footer.vue'

export default {
  components: {
    'Games-Cards': Cards,
    'index-Footer': Footer
  },
  data() {
    return {
    }
  }
}
</script>
<style scoped lang="scss">
</style>
