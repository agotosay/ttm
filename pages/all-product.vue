<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <section>
      <b-container>
        <!-- 1 -->
        <b-row class="acc-product">
          <b-col cols="6" class="hammock left">
            <div class="title">HAMMOCKS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner" v-on:click="isHidden1 = !isHidden1">
              SEE ALL HAMMOCKS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="collapse-acc-product d-flex align-items-center" v-if="isHidden1">
          <b-col cols="6 mb-2">
            <div class="our-products">
              <img
              class="d-block img-fluid w-100"
              src="/product-1.jpg"
              alt="image"
              />
              <div class="product-title mb-1">
                TRAVEL HAMMOCK
              </div>
              <div class="product-rating">
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
              </div>
              <div class="product-price">40.99 &euro;</div>
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2 radius-corner" @click="$router.push('/detail-product')">
                SHOP NOW
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
          <b-col cols="6 mb-2">
            <div class="our-products">
              <img
              class="d-block img-fluid w-100"
              src="/product-1.jpg"
              alt="image"
              />
              <div class="product-title mb-1">
                TRAVEL HAMMOCK
              </div>
              <div class="product-rating">
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
              </div>
              <div class="product-price">40.99 &euro;</div>
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2 radius-corner" @click="$router.push('/detail-product')">
                SHOP NOW
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
          <b-col cols="6 mb-2">
            <div class="our-products">
              <img
              class="d-block img-fluid w-100"
              src="/product-1.jpg"
              alt="image"
              />
              <div class="product-title mb-1">
                TRAVEL HAMMOCK
              </div>
              <div class="product-rating">
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
                <i class="fas fa-star text-warning"></i>
              </div>
              <div class="product-price">40.99 &euro;</div>
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2 radius-corner" @click="$router.push('/detail-product')">
                SHOP NOW
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
          <b-col cols="6 mb-2">
            <div class="our-products">
              <div class="text-center fw-900">SEE OTHER PRODUCT</div>
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2 radius-corner" @click="$router.push('/detail-product')">
                VIEW MORE
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
        </b-row>
        <!-- 2 -->
        <b-row class="acc-product">
          <b-col cols="6" class="chairs left">
            <div class="title">HAMMOCKS CHAIRS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner">
              SEE ALL CHAIRS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-32.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="backpacks left">
            <div class="title">ECO BACKPACKS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner">
              SEE ALL BACKPACKS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-33.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="bags left">
            <div class="title">ECOBAGS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner">
              SEE ALL BAGS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-34.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="accessories left">
            <div class="title">HAMMOCK ACCESSORIES</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner">
              SEE ALL ACCESSORIES
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-35.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="suspension left">
            <div class="title">HAMMOCK SUSPENSION</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner">
              SEE ALL SUSPENSION
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-36.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="tools left">
            <div class="title">TOOLS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner">
              SEE ALL TOOLS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-37.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="others left">
            <div class="title">OTHERS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100 radius-corner">
              SEE ALL OTHERS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </b-col>
          <b-col cols="6" class="right pl-0">
            <img
            class="d-block img-fluid w-100"
            src="/image-38.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
      </b-container>
    </section>

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
        isHidden1: false
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
