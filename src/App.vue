<template>
  <div>
    <Navbar class="sticky"/>
    <Hero />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    Footer
  }
}
</script>
<style scoped>
.sticky {
  position: sticky;
  top: 0;
  z-index: 3;
}
</style>

