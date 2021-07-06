<template>
  <div>
    <!-- top bar -->
    <div class="top-bar">
      <b-nav pills>
        <b-nav-item-dropdown
        id="my-nav-dropdown"
        text="EN"
        toggle-class="nav-link-custom"
        right
      >
        <b-dropdown-item>One</b-dropdown-item>
        <b-dropdown-item>Two</b-dropdown-item>
        <b-dropdown-divider></b-dropdown-divider>
        <b-dropdown-item>Three</b-dropdown-item>
        </b-nav-item-dropdown>
        <b-nav-item-dropdown
          id="my-nav-dropdown"
          text="EUR"
          toggle-class="nav-link-custom"
          right
        >
          <b-dropdown-item>One</b-dropdown-item>
          <b-dropdown-item>Two</b-dropdown-item>
          <b-dropdown-divider></b-dropdown-divider>
          <b-dropdown-item>Three</b-dropdown-item>
        </b-nav-item-dropdown>
        <b-nav-item>Link</b-nav-item>
      </b-nav>
    </div>

    <!-- navbar -->
    <b-navbar toggleable="lg" type="light" variant="light">
      <b-navbar-brand href="#">TICKETTOTHEMOON</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown text="PRODUCTS" right>
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item href="#">SHOP</b-nav-item>
          <b-nav-item href="#">BUNDLES</b-nav-item>
          <b-nav-item href="#">ABOUT US</b-nav-item>
          <b-nav-item href="#">GALLERY</b-nav-item>
          <b-nav-item href="#">CONTACT</b-nav-item>
          <b-nav-item href="#">
            <b-img src="../static/shopping-bag.svg" fluid alt="" width="14"></b-img>
          </b-nav-item>

        </b-navbar-nav>
      </b-collapse>
    </b-navbar>

    <!-- carousel -->
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="700"
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
              src="/bc-1.jpg"
              alt="image"
            />
           <b-container>
              <div class="slide-wording position-absolute">
                <h1>INTRODUCING:</h1>
                <h1>THE PRO HAMMOCK</h1>
                <b-row>
                  <b-col cols="9">
                    <p>Design as an easy-to-use and always-ready solution with ridge-line and insect protection</p>
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
              src="/bc-1.jpg"
              alt="image"
            />
           <b-container>
              <div class="slide-wording position-absolute">
                <h1>INTRODUCING:</h1>
                <h1>THE PRO HAMMOCK</h1>
                <b-row>
                  <b-col cols="9">
                    <p>Design as an easy-to-use and always-ready solution with ridge-line and insect protection</p>
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

    <!-- img separator -->
    <div class="img-separator">
      <img
        class="d-block w-100 img-margin"
        height="600"
        src="/img-1.png"
        alt="image"
      />
    </div>

    <!-- travel hammock -->
    <section>
      <b-container class="text-center">
        <div class="title">
          TRAVEL HAMMOCK
        </div>
        <img
          class="d-block img-fluid img-margin"
          src="/img-2.png"
          alt="image"
        />
        <b-row>
          <b-col cols="6" offset-md="3">
            <p>In publishing and graphic design, Lorem ipsum placeholder text commonly used to demonstrate the visual form of a document typeface without relying on meaningful content. Lorem ipsum may be used as</p>
          </b-col>
        </b-row>
        <b-link href="#">
          SEE ALL HAMMOCK
          <img 
            src="/arrow-right.svg" 
            width="6"
            alt="image" 
            class="ml-1" 
          />
        </b-link>
      </b-container>
    </section>

    <!-- find store -->
    <section class="find-store">
      <b-row class="mr-0 ml-0">
        <b-col cols="3" 
          height="300" 
          class="left-content pl-0 pr-0 text-center">
          <div>
            <div class="text-center content">
              FIND A <br /><span class="fw-900">STORE</span><br /> IN YOUR <br /><span class="fw-900">LOCATION</span>
            </div>
            <b-link href="#" class="d-block mt-2">
              SEE PRODUCTS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" 
              />
            </b-link>
          </div>
        </b-col>
        <b-col cols="9" class="pl-0 pr-0">
          <img
          class="d-block img-fluid w-100"
          height="300"
          src="/img-3.png"
          alt="image"
          />
        </b-col>
      </b-row>
    </section>

    <!-- products -->
    <section class="our-product">
      <b-container>
        <div class="title text-center">
          OUR PRODUCTS
        </div>
        <b-row class="mt-2">
          <b-col cols="3" v-for="(item, index) in ourProduct" :key="index">
            <img
            class="d-block img-fluid w-100"
            :src="item.image.url"
            alt="image"
            />
            <div class="product-title mb-1">
              {{ item.name }}
            </div>
            <div class="product-rating">
              <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= item.rating}"></i>
            </div>
            <div class="product-price">19.99 &euro;</div>
          </b-col>
        </b-row>
        <b-link href="#" class="d-block mt-3 text-center">
          VIEW ALL PRODUCTS
          <img 
            src="/arrow-right.svg" 
            width="6"
            alt="image" 
            class="ml-1" 
          />
        </b-link>
      </b-container>
    </section>

     <!-- review -->
     <section class="reviews">
      <b-container>
        <div class="title text-center">
          REVIEWS
        </div>
        <div>
          <VueSlickCarousel :arrows="true" :dots="true">
            <div>1</div>
            <div>2</div>
            <div>3</div>
            <div>4</div>
          </VueSlickCarousel>
        </div>
      </b-container>
     </section>
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Alegreya+Sans:wght@300;400;500;900&display=swap");
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css");
</style>

<script>
import VueSlickCarousel from 'vue-slick-carousel'

export default {
  name: 'MyComponent',
  components: { VueSlickCarousel },

  data() {
      return {
        slide: 0,
        sliding: null,
        ourProduct: [
          {
            id: 1,
            name: 'Travel Hammocks',
            image: {
              url: '/product-1.jpg'
            },
            price: '19.99',
            rating: 5,
          },
          {
            id: 2,
            name: 'Backpack Plus 25 L',
            image: {
              url: '/product-2.jpg'
            },
            price: '19.99',
            rating: 2,
          },
          {
            id: 3,
            name: 'Pro Hammock',
            image: {
              url: '/product-3.jpg'
            },
            price: '19.99',
            rating: 3,
          },
          {
            id: 4,
            name: 'Backpack Plus 10 L',
            image: {
              url: '/product-4.jpg'
            },
            price: '19.99',
            rating: 4,
          }
        ]
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
