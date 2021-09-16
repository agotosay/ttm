<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
    <div class="static-info">
      <!-- carousel -->
      <div class="position-relative">
        <b-carousel v-bind="mainCarousel"
          id="carousel-1"
          v-model="slide"
          :interval="4000"
          indicators
          @sliding-start="onSlideStart"
          @sliding-end="onSlideEnd"
        >
          <!-- Text slides with image -->
          <b-carousel-slide>
            <template #img>
              <div class="slide-banner position-relative">
                <img
                  class="d-block w-100 img-auto"
                  height="700"
                  src="/banner1.jpg"
                  alt="image"
                />
              <b-container>
                <div class="slide-wording position-absolute text-center mt-2">
                  <h1>INTRODUCING: <span class="fw-900">THE PRO HAMMOCK</span></h1>
                  <b-row>
                    <b-col cols="12" lg="10" offset="1">
                        <p>I was blown away by the tiny packing size and the very thin and light material. It certainly lightest hammock I have ever come across. The material feels like very fine silk.</p>
                    </b-col>
                  </b-row>
                  <b-button variant="primary" class="mt-2">
                    SHOP NOW
                    <img 
                      src="/arrow-right.svg" 
                      width="6"
                      alt="image" 
                      class="ml-1" />
                  </b-button>
                </div>
              </b-container>
              </div>
            </template>
          </b-carousel-slide>
          <b-carousel-slide>
            <template #img>
              <div class="slide-banner position-relative">
                <img
                  class="d-block w-100 img-auto"
                  height="700"
                  src="/banner1.jpg"
                  alt="image"
                />
              <b-container>
                <div class="slide-wording position-absolute text-center mt-2">
                  <h1>INTRODUCING: <span class="fw-900">THE PRO HAMMOCK</span></h1>
                  <b-row>
                    <b-col cols="12" lg="10" offset="1">
                        <p>I was blown away by the tiny packing size and the very thin and light material. It certainly lightest hammock I have ever come across. The material feels like very fine silk.</p>
                    </b-col>
                  </b-row>
                  <b-button variant="primary" class="mt-2">
                    SHOP NOW
                    <img 
                      src="/arrow-right.svg" 
                      width="6"
                      alt="image" 
                      class="ml-1" />
                  </b-button>
                </div>
              </b-container>
              </div>
            </template>
          </b-carousel-slide>
        </b-carousel>
        <div class="badge-fast">
          <b-link href="">FASTEST<br />SHIPPING!</b-link>  
        </div>
      </div>

      <section>
        <b-container class="bundles">
          <div class="title mb-1">BUNDLES</div>
          <p>Our hammock sets are the perfect choice for starters or seasoned adventurers looking to upgrade their existing equipment.</p>
          <b-row>
            <b-col cols="12" lg="6">
              <div class="info bc-yellow text-center mb-2">
                <div class="title">Lightest Hammock <br />BUNDLE</div>
                <p class="mb-1">I was blown away by the tiny packing size and the very thin and light material. It certainly lightest hammock I have ever come across.</p>
                <b-button variant="secondary" class="mt-1 w-100 rounded-radius">
                  SEE BUNDLE
                  <img 
                    src="/arrow-right.svg" 
                    width="6"
                    alt="image" 
                    class="ml-1" />
                </b-button>
              </div>
            </b-col>
            <b-col cols="12" lg="6">
              <div class="info backpacks text-center mb-2">
                <div class="title">Hammock <br />Tent Set</div>
                <p class="mb-1">I was blown away by the tiny packing size and the very thin and light material. It certainly lightest hammock I have ever come across.</p>
                <b-button variant="secondary" class="mt-1 w-100 rounded-radius">
                  SEE TENT SET
                  <img 
                    src="/arrow-right.svg" 
                    width="6"
                    alt="image" 
                    class="ml-1" />
                </b-button>
              </div>
            </b-col>
          </b-row>
          <p class="text-center">Our Ticket To The Moon (TTTM) Hammock Bundles Are The Perfect Choices For Aspiring Hammockers And Experienced Adventurers Looking To Upgrade Their Existing Gear. These Popular Sets Make Relaxation Easier Than Ever, Wherever Your Travels Take You. We Offer 5 Bundles Depending On Your Unique Needs. While Other Options May Compromise On Functionality, TTTM Sets Include All Essential Accessories For Many Exciting Hangs To Come. Our Hammock Tent Set And Lightest Hammock Bundle Are Convenient And Fully-featured. They’re Also Affordable – You Won’t Have To Break The Bank Or Worry About Added Shipping Costs.</p>
        </b-container>
      </section>
    </div>

    <!-- footer -->
    <Footer />
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Alegreya+Sans:wght@300;400;500;600;900&display=swap");
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css");
</style>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import TopNavbar from'/components/top-navbar'
import Footer from'/components/footer'
import Navbar from'/components/navbar'

export default {
  name: 'MyComponent',
  components: { 
    VueSlickCarousel,
    TopNavbar,
    Footer,
    Navbar
  },

  data() {
      return {
        slide: 0,
        sliding: null,
        isHidden: false,
        mainCarousel: {
          indicators: true,
          background: "#e2ecf3",
        }
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
}
</script>
