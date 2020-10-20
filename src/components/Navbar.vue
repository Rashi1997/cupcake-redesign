<template>
  <div>
    <Notification />
    <b-navbar toggleable="md" type="light" variant="white">
      <b-navbar-brand href="#" class="logo">
        <img src="../assets/logo.png" width="50" height="50" alt="toronto cupcake logo">
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav class="collapse">
        <b-navbar-nav class="ml-auto">

          <b-input-group>
            <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          </b-input-group>
        </b-navbar-nav>
        <b-navbar-nav>

          <div class="columns custom-nav">

            <div class="column">
              <b-nav-item href="#">
                <cupcake />
                <span>Flavors</span>
              </b-nav-item>
            </div>

          </div>
          <div class="columns custom-nav">

            <div class="column">
              <b-nav-item href="#">
                <pin />
                <span>Stores</span>
              </b-nav-item>
            </div>

          </div>
          <div class="columns custom-nav">

            <div class="column">
              <b-nav-item href="#">
                <cart />
                <span>Cart</span>
              </b-nav-item>
            </div>

          </div>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>

    <b-navbar toggleable="lg" type="light" variant="white" sticky>
      <b-navbar-toggle target="navbar-toggle-menu" class="ml-auto">
        <template #default="{ expanded }">
          <b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
          <b-icon v-else icon="chevron-bar-down"></b-icon>
        </template>
      </b-navbar-toggle>

      <b-collapse id="navbar-toggle-menu" is-nav>
        <b-navbar-nav class="m-auto">
          <b-nav-item>HALLOWEEN</b-nav-item>
          <b-nav-item>CUPCAKES</b-nav-item>
          <b-nav-item>TREATS</b-nav-item>
          <b-nav-item>BIRTHDAY</b-nav-item>
          <b-nav-item>GIFTING OCCASIONS</b-nav-item>
          <b-nav-item>PICK YOUR OWN</b-nav-item>
          <b-nav-item>CORPORATE GIFTS & EVENTS</b-nav-item>
          <b-nav-item>FAQS</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
import Notification from './Notification.vue'
import cupcake from './cupcake.vue'
import pin from './pin.vue'
import cart from './cart.vue'

export default {
  name: 'Navbar',
  components: {
    cupcake,
    pin,
    cart,
    Notification
  }
}
</script>

<style scoped>
.custom-nav a {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
}

.custom-nav i {
  font-size: 3rem;
}

.collapse {
  padding-right: 400px;
}
.logo {
  padding-left: 400px;
}
.nav-link {
  border-bottom: 3px solid white;
  font-weight: 700;
}
.nav-link:hover {
  border-bottom: 3px solid var(--dark_hue);
}

@media only screen and (min-width: 375px) {
  .collapse {
    padding-right: 0;
  }
  .logo {
    padding-left: 0;
  }
}

@media only screen and (min-width: 768px) {
  .collapse {
    padding-right: 100px;
  }
  .logo {
    padding-left: 100px;
  }
}
</style>
