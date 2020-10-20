<template>
  <footer>
    <div class="desktop marginator">

      <section class="align-center first">
        <img src="../assets/logo.png" width="90" height="90" alt="toronto cupcake logo">
        <h1 class="ml-4 display-4 font-weight-bold">Toronto Cupcake</h1>
        <div id="give-to-brown" class="ml-auto">
         <b-button href="#" class="giving-footer" variant="more" size="lg">Giving Back</b-button>
        </div>
      </section>
      <b-row class="second"> 
        <b-col>
          <b-row><h1 class="mb-5">ABOUT</h1></b-row>
          <b-row><b-link class="link" href="#"><u>Our Story</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Flavor Menu</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Collaborations</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Locations</u></b-link></b-row>
        </b-col>
        <b-col>
          <b-row><h1 class="mb-5">HELP</h1></b-row>
          <b-row><b-link class="link" href="#"><u>FAQs</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Resources</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Contact Us</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Shipping & Delivery</u></b-link></b-row>
        </b-col>
        <b-col>
          <b-row class="link"><b-icon-map></b-icon-map><h5 class="link">Toronto, Canada</h5></b-row>
          <b-row class="link"><b-icon-telephone-fill></b-icon-telephone-fill><h5 class="ml-2">
            <span class="link"><u>647-478-9464</u></span>
            </h5></b-row>
          <b-row class="link"><b-icon-clock-history></b-icon-clock-history><h5 class="ml-2">
            <span class="link">
            &nbsp;&nbsp;Monday - Saturday:&nbsp;&nbsp;
            &nbsp;&nbsp;7am - 10pm<br>
            &nbsp;&nbsp;Sunday:&nbsp;&nbsp;
            &nbsp;&nbsp;7am - 10pm(no pick ups, deliveries for 2doz or more)  
            </span>
          </h5></b-row>
          <b-row class="link"><b-icon-envelope-fill></b-icon-envelope-fill><h5 class="ml-2">
            <b-link href="inquiry@torontocupcake.com" class="link" disabled>inquiry@torontocupcake.com</b-link>
            </h5></b-row>
        </b-col>
      </b-row>
      <section class="third text-right">Copyright 2020 @ Rashi Dhar</section>
    </div>

    <div class="mobile mobile-styles">

      <section class="align-center">
        <img src="../assets/logo.png" width="90" height="90" alt="toronto cupcake logo">
        <h1 class="ml-4 font-weight-bold">Toronto Cupcake</h1>
      </section>
      <section class="align-center m-first">
        <div id="give-to-brown">
         <b-button href="#" class="giving-footer" variant="more" size="lg">Giving Back</b-button>
        </div>
      </section>
      <b-row class="second"> 
        <b-col>
          <b-row><h1 class="mb-5 mr-5">ABOUT</h1></b-row>
          <b-row><b-link class="link" href="#"><u>Our Story</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Flavor Menu</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Collaborations</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Locations</u></b-link></b-row>
        </b-col>
        <b-col>
          <b-row><h1 class="mb-5">HELP</h1></b-row>
          <b-row><b-link class="link" href="#"><u>FAQs</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Resources</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Contact Us</u></b-link></b-row>
          <b-row><b-link class="link" href="#"><u>Shipping & Delivery</u></b-link></b-row>
        </b-col>
      </b-row>
      <b-row class="second">
        <b-col>
          <b-row class="link"><b-icon-map></b-icon-map><h5 class="link">Toronto, Canada</h5></b-row>
          <b-row class="link"><b-icon-telephone-fill></b-icon-telephone-fill><h5 class="ml-2">
            <span class="link"><u>647-478-9464</u></span>
            </h5></b-row>
          <b-row class="link"><b-icon-clock-history></b-icon-clock-history><h5 class="ml-2">
            <span class="link">
            &nbsp;&nbsp;Monday - Saturday:&nbsp;&nbsp;
            &nbsp;&nbsp;7am - 10pm<br>
            &nbsp;&nbsp;Sunday:&nbsp;&nbsp;
            &nbsp;&nbsp;7am - 10pm(no pick ups, deliveries for 2doz or more)  
            </span>
          </h5></b-row>
          <b-row class="link"><b-icon-envelope-fill></b-icon-envelope-fill><h5 class="ml-2">
            <b-link href="inquiry@torontocupcake.com" class="link" disabled>inquiry@torontocupcake.com</b-link>
            </h5></b-row>
        </b-col>
      </b-row>
      <section class="third text-right">Copyright 2020 @ Rashi Dhar</section>
    </div>
  </footer>
</template>

<script>
// import phone from './phone.vue'
// import time from './time.vue'
// import mail from './mail.vue'

export default {
  name: 'Footer'
}
</script>

<style scoped>
.mobile {
  display: none;
}
.desktop {
  display: block;
}
.marginator {
  background-color: var(--dark_hue);
  color: white;
  margin: auto;
  padding: 60px;
}
.align-center {
  display: flex;
  justify-content: center;
  align-content: center;
}
.first {
  padding: 50px;
  padding-bottom: 20px;
  width: 90vw;
  border-bottom: 0.1rem solid white;
}
.second {
  padding: 25px;
  width: 90vw;
  border-bottom: 0.1rem solid white;
}
.third {
  padding-top: 10px;
  padding-left: 50px;
  padding-right: 50px;
  width: 90vw;
}
.link {
  color: white;
  padding-bottom: 0.5rem;
  padding-left: 1rem;
}
@media only screen and (max-width: 375px) {
  .mobile {
    display: block;
  }
  .desktop {
    display: none;
  }
  .third {
    text-align: center;
    padding-bottom: 10px;
  }
}

@media only screen and (min-width: 768px) {
  .second {
    padding: 40px;
  }
}
.mobile-styles {
  background-color: var(--dark_hue);
  color: white;
  margin: auto;
  padding-left: 25px;
  padding-right: 25px;
  padding-top: 30px;
}
.m-first {
  padding-bottom: 20px;
  padding-top: 20px;
  border-bottom: 0.1rem solid white;
}
</style>

