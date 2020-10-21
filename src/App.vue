<template>
  <div>
    <Navbar class="sticky"/>
    <Hero />
    <Products />
    <CustomDesign />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import Footer from './components/Footer.vue'
import Products from './components/Products.vue'
import CustomDesign from './components/CustomDesign.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    Footer,
    Products,
    CustomDesign
  }
}
</script>
<style scoped>
.sticky {
  position: sticky;
  top: 0;
  z-index: 30;
}
</style>

