<template>
  <div>
    <Notification />
    <Navbar />
  </div>
</template>

<script>
import Notification from './components/Notification.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'App',
  components: {
    Notification,
    Navbar
  }
}
</script>

