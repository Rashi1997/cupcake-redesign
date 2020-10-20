<template>
  <div>
    <b-navbar toggleable="md" type="light" variant="white">
      <b-navbar-brand href="#" class="logo">
        <img src="../assets/logo.png" width="100" height="100" alt="toronto cupcake logo">
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav class="collapse">
        <b-navbar-nav class="ml-auto">

          <b-input-group>
            <b-form-input size="md" class="mr-sm-2" placeholder="Search"></b-form-input>
            <b-input-group-append>
              <b-input-group-text>
                <b-icon-search></b-icon-search>
              </b-input-group-text>
            </b-input-group-append>
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
  </div>
</template>

<script>

import cupcake from './cupcake.vue'
import pin from './pin.vue'
import cart from './cart.vue'

export default {
  name: 'Navbar',
  components: {
    cupcake,
    pin,
    cart
  }
}
</script>

<style scoped>
.custom-nav a {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
  padding: 1em;
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

@media only screen and (max-width: 375px) {
  .collapse {
    padding-right: 0;
  }
  .logo {
    padding-left: 0;
  }
}

@media only screen and (max-width: 768px) {
  .collapse {
    padding-right: 100px;
  }
  .logo {
    padding-left: 100px;
  }
}
</style>
