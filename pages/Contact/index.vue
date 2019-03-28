<template>
  <div class="contactpage">
    <div class="title">
      <h1>Contact</h1>
      <div class="stripe"></div>
      <Contact-Email />
      <Contact-Social />
    </div>
    <Contact-Verantwoording />
    <index-Footer />
  </div>
</template>

<script>
import Email from '@/components/Contact/Email.vue'
import Social from '@/components/Contact/Social.vue'
import Verantwoording from '@/components/Contact/Verantwoording.vue'
import Footer from '@/components/Footer.vue'
export default {
  components: {
    'Contact-Email': Email,
    'Contact-Social': Social,
    'Contact-Verantwoording': Verantwoording,
    'index-Footer': Footer
  },
  data() {
    return {
    }
  }
}
</script>
<style scoped lang="scss">
  .contactpage {
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
