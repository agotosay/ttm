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

    <section>
      <b-container>
        <!-- 1 -->
        <b-row class="acc-product">
          <b-col cols="6" class="hammock left">
            <div class="title">HAMMOCKS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100" v-on:click="isHidden1 = !isHidden1">
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
            src="/image 19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="collapse-acc-product" v-if="isHidden1">
          <b-col cols="4">
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
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="$router.push('/detail-product')">
                SHOP NOW
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
          <b-col cols="4">
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
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="$router.push('/detail-product')">
                SHOP NOW
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
          <b-col cols="4">
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
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="$router.push('/detail-product')">
                SHOP NOW
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
            <b-button variant="secondary" class="mt-1 w-100">
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
            src="/image 19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="backpacks left">
            <div class="title">ECO BACKPACKS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100">
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
            src="/image 19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="bags left">
            <div class="title">ECOBAGS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100">
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
            src="/image 19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="accessories left">
            <div class="title">HAMMOCK ACCESSORIES</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100">
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
            src="/image 19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="suspension left">
            <div class="title">HAMMOCK SUSPENSION</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100">
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
            src="/image 19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="tools left">
            <div class="title">TOOLS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100">
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
            src="/image 19.png"
            alt="image"
            height="218"
            />
          </b-col>
        </b-row>
        <b-row class="acc-product">
          <b-col cols="6" class="others left">
            <div class="title">OTHERS</div>
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. </p>
            <b-button variant="secondary" class="mt-1 w-100">
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
            src="/image 19.png"
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
