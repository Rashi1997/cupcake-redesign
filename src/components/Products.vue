<template>
  <div class="trendtreats">
    <b-container fluid>
      <b-row class="mb-5 tab">
        <h1 class="big-text align-center text-center">TRENDING TREATS</h1>
        <h3 class="text align-center text-center">BEST SELLING TREATS & GIFT BOXES</h3>
      </b-row>
      <b-row class="mb-5 mobile">
        <h1 class="big-text align-center text-center">TRENDING TREATS</h1>
        <h3 class="text align-center text-center">BEST SELLING TREATS & GIFT BOXES</h3>
      </b-row>
      <b-row>
        <b-col md="3" lg="3" class="trending text-left desktop">
          <br><br><br><br><br>
          <h1 class="big-text align-center text-left">TRENDING TREATS</h1>
          <h3 class="text align-center text-left">BEST SELLING TREATS & GIFT BOXES</h3>
        </b-col>
        <b-col class="cards desktop">
          <div>
            <b-carousel
              id="carousel-1"
              v-model="slide"
              :interval="4000"
              controls
              indicators
              background="#ababab"
              img-width="1024"
              img-height="1025"
              style="color: black"
              @sliding-start="onSlideStart"
              @sliding-end="onSlideEnd"
            >

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/download.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/chocolatehazelnut.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/CanadaDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.26</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/chocolateoreo.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.24</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                  <b-card :img-src="require('../assets/ChocolateVanilla.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$4.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/download.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/Easter.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.75</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/Face.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.98</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/lemon_vanilla.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.45</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                  <b-card :img-src="require('../assets/PrideDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/download.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/redvelvetfudge.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.05</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/StPatricksDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$4.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/vanillachocolateganache.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.21</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                  <b-card :img-src="require('../assets/VanillaStrawberry.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.99</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

            </b-carousel>
          </div>
        </b-col>

        <b-col class="cards tab">
          <div>
            <b-carousel
              id="carousel-1"
              v-model="slide"
              :interval="4000"
              controls
              indicators
              background="#ababab"
              img-width="1024"
              img-height="1025"
              style="color: black"
              @sliding-start="onSlideStart"
              @sliding-end="onSlideEnd"
            >

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/download.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/chocolatehazelnut.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/CanadaDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.26</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/chocolateoreo.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.24</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                  <b-card :img-src="require('../assets/ChocolateVanilla.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$4.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/download.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/Easter.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.75</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/Face.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.98</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/lemon_vanilla.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.45</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                  <b-card :img-src="require('../assets/PrideDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/download.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/redvelvetfudge.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.05</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/StPatricksDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$4.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>

                  <b-card :img-src="require('../assets/vanillachocolateganache.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.21</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                  <b-card :img-src="require('../assets/VanillaStrawberry.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.99</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

            </b-carousel>
          </div>
        </b-col>
        
        <b-col class="cards mobile">
          <div>
            <b-carousel
              id="carousel-1"
              v-model="slide"
              :interval="1000000"
              controls
              indicators
              background="#ababab"
              img-width="1024"
              img-height="1025"
              style="color: black"
              @sliding-start="onSlideStart"
              @sliding-end="onSlideEnd"
            >

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/chocolatehazelnut.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>

              <b-carousel-slide :img-src="require('../assets/mobile.svg')">

                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/CanadaDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.26</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>

              <b-carousel-slide :img-src="require('../assets/mobile.svg')">

                <b-card-group deck style="color:black;">

                  <b-card :img-src="require('../assets/chocolateoreo.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.24</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>

              <b-carousel-slide :img-src="require('../assets/mobile.svg')">

                <b-card-group deck style="color:black;">
                  
                  <b-card :img-src="require('../assets/ChocolateVanilla.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$4.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/Easter.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.75</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>

              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/Face.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.98</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>

              
              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/lemon_vanilla.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.45</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>


              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/PrideDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

              <!-- Slides with custom text -->
              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/redvelvetfudge.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.05</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>

              
              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/StPatricksDay.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$4.25</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>


              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/vanillachocolateganache.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.21</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                </b-card-group>
              </b-carousel-slide>

              
              <b-carousel-slide :img-src="require('../assets/mobile.svg')">
                
                <b-card-group deck style="color:black;">
                  <b-card :img-src="require('../assets/VanillaStrawberry.jpg')" img-alt="Image" img-top>
                    <b-card-text>
                      <span>$3.99</span>
                    </b-card-text>
                    <template #footer>
                      <b-button variant="dark_hue">SHOP</b-button>
                    </template>
                  </b-card>
                  
                </b-card-group>

              </b-carousel-slide>

            </b-carousel>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slide: 0,
      sliding: null
    }
  },
  methods: {
    onSlideStart() {
      this.sliding = true
    },
    onSlideEnd() {
      this.sliding = false
    }
  },
  name: 'Products'
}
</script>

<style scoped>

  .carousel-control-next-icon,
  .carousel-control-prev-icon {
    filter: invert(1);
  }
  .tab {
    display: block;
    color: black;
  }
  .desktop {
    display: none;
  }
  .mobile {
    display: none;
  }
  .show {
    display: none;
  }
  .trendtreats{
    margin-top: 100px;
    margin-bottom: 30px;
    color: white;
    height: 70vh;
  }
  .cards {
    max-height: 100vh;
  }
  .text {
    font-size: 1rem;
    font-weight: 500;
  }
  .big-text {
    font-weight: 700;
  }
  
@media only screen and (max-width: 375px) {
  .mobile {
    display: block;
    color: black;
  }
  .show {
    display: block;
  color: black;
  }
  .tab {
    display: none;
  }
  .desktop {
    display: none;
  }
  .tablet {
    display: none;
  }
  .text {
    font-size: 1rem;
    font-weight: 500;
  }
  .big-text {
    font-weight: 700;
  }
  .trendtreats{
    margin-top: 100px;
    margin-bottom: 30px;
    color: white;
    height: 100%;
  }
  .cards {
    padding-top: 8px;
  }
}

@media only screen and (min-width: 780px) {
  .show {
    display: none;
    height: 100%;
  }
  .desktop {
    display: block;
  }
  .tablet {
    display: none;
  }
  .mobile {
    display: none;
  }
  .tab {
    display: none;
  }

  .align-center {
    display: flex;
    justify-content: center;
    align-content: center;
  }
  .trendtreats{
    margin-top: 100px;
    margin-bottom: 50px;
    color: white;
    height: 100%;
  }
  .trending {
    max-width: 40vw;
    background-color: var(--dark_hue);
  }
  .text {
    font-weight: 500;
  }
  .big-text {
    font-weight: 700;
  }
}

/* @media only screen and (max-width: 768px) {
} */
</style>

