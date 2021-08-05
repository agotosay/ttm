<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <div class="position-relative top-bar">
      <b-navbar toggleable="lg" type="light" variant="light">
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" class="justify-content-between" is-nav>
          <!-- Right aligned nav items -->
          <div class="input-group search">
            <div class="input-group-prepend">
              <img
              class="ml-1"
              src="/loupe.svg"
              height="14"
              alt="image"
              />
            </div>
            <input type="text" class="form-control" placeholder="" aria-label="Username" aria-describedby="basic-addon1">
          </div>
          <b-navbar-nav>
            <b-nav-item class="link-icon" href="#" v-on:click="isHidden = !isHidden">
              PRODUCTS
              <img
              class="ml-1"
              src="/arrow-down.svg"
              height="10"
              alt="image"
              />
            </b-nav-item>
            <b-nav-item href="#" @click="$router.push('/bundles')">BUNDLES</b-nav-item>
            <b-nav-item href="#" @click="$router.push('/about-us')">ABOUT US</b-nav-item>
            <b-nav-item href="#" @click="$router.push('/gallery')">GALLERY</b-nav-item>
            <b-nav-item href="#" class="ml-0" @click="$router.push('/contact-us')">CONTACT</b-nav-item>

          </b-navbar-nav>
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
            <b-nav-item class="user">
              <img
              class="d-block img-margin"
              height="14"
              src="/cart.png"
              alt="image"
              />
            </b-nav-item>
            <b-nav-item class="user" @click="$router.push('/signIn')">
              <img
              class="d-block img-margin"
              height="14"
              src="/user.svg"
              alt="image"
              />
            </b-nav-item>
          </b-nav>
        </b-collapse>
      </b-navbar>

      <div class="mega-menu" v-if="isHidden">
        <b-container>
          <b-row>
            <b-col cols="3">
              <div class="title">Hammock</div>
              <ul>
                <li>
                  <b-link>
                    Travel Hammock
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Lightest Hammock
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Pro Hammock
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="3">
              <div class="title">Hammock Chair</div>
              <ul>
                <li>
                  <b-link>
                    Moon Chair
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Mini Moon Chair
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="3">
              <div class="title">Eco Backpack</div>
              <ul>
                <li>
                  <b-link>
                    Mini Backpack 15 L
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Backpack Plus 25 L
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="3">
              <div class="title">Eco Shopping Bag</div>
              <ul>
                <li>
                  <b-link>
                    Eco Bags
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
          </b-row>
          <b-row class="mt-2">
            <b-col cols="3">
              <div class="title">Hammock Accessories</div>
              <ul>
                <li>
                  <b-link>
                    UV-Proof Hammock Sleeve
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Convertiblebug Net 360º
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Moonquilt
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Moontrap
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Fuul Moon Traap
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Lightest Trap
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="3">
              <div class="title">Hammock Suspension</div>
              <ul>
                <li>
                  <b-link>
                    Moon Straps
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Lightest Strap
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Nautical Rope Kit
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="3">
              <div class="title">Tools</div>
              <ul>
                <li>
                  <b-link>
                    Carabiner 10 KN
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    Carabiner 22 KN
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    HAMMOCK ANCHOR KIT
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    RIDGELINE KIT
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="3">
              <div class="title">OTHERS</div>
              <ul>
                <li>
                  <b-link>
                    POCKET FRISBEE
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    BEACH BLANKET
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
                <li>
                  <b-link>
                    SLACKLINE
                    <img
                    class="ml-1"
                    src="/arrow-right.svg"
                    height="12"
                    alt="image"
                    />
                  </b-link>
                </li>
              </ul>
            </b-col>
          </b-row>
        </b-container>
      </div>
    </div>

    <!-- info -->
    <div class="static-info">
      <!-- carousel -->
      <!-- carousel -->
      <div class="position-relative">
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
                  src="/banner1.jpg"
                  alt="image"
                />
              <b-container>
                <div class="slide-wording position-absolute text-center mt-2">
                  <h1>INTRODUCING: <span class="fw-900">THE PRO HAMMOCK</span></h1>
                  <b-row>
                    <b-col cols="10" offset="1">
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
            <b-col cols="6">
              <div class="info bc-yellow text-center mb-2">
                <div class="title">Lightest Hammock <br />BUNDLE</div>
                <p class="mb-1">I was blown away by the tiny packing size and the very thin and light material. It certainly lightest hammock I have ever come across.</p>
                <b-button variant="secondary" class="mt-1 w-100">
                  SEE BUNDLE
                  <img 
                    src="/arrow-right.svg" 
                    width="6"
                    alt="image" 
                    class="ml-1" />
                </b-button>
              </div>
            </b-col>
            <b-col cols="6">
              <div class="info backpacks text-center mb-2">
                <div class="title">Hammock <br />Tent Set</div>
                <p class="mb-1">I was blown away by the tiny packing size and the very thin and light material. It certainly lightest hammock I have ever come across.</p>
                <b-button variant="secondary" class="mt-1 w-100">
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

export default {
  name: 'MyComponent',
  components: { 
    VueSlickCarousel,
    TopNavbar,
    Footer
  },

  data() {
      return {
        slide: 0,
        sliding: null,
        isHidden: false
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
