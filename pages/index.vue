<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <div class="position-relative">
      <b-navbar toggleable="lg" type="light" variant="light">
        <b-navbar-brand @click="$router.push('/')" class="logo">
          <img
          class="d-block img-margin"
          src="/black-logo.png"
          height="20"
          alt="image"
          />
        </b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="#" v-on:click="isHidden = !isHidden">PRODUCTS</b-nav-item>
            <b-nav-item href="#">SHOP</b-nav-item>
            <b-nav-item href="#">BUNDLES</b-nav-item>
            <b-nav-item href="#">ABOUT US</b-nav-item>
            <b-nav-item href="#">GALLERY</b-nav-item>
            <b-nav-item href="#">CONTACT</b-nav-item>
            <b-nav-item to="/signIn">
              <b-img src="../static/shopping-bag.svg" fluid alt="" width="14"></b-img>
            </b-nav-item>

          </b-navbar-nav>
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
      <div class="badge-fast">
        <b-link href="">FASTEST<br />SHIPPING!</b-link>  
      </div>
    </div>

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
          <b-col cols="3" v-for="(item, index) in ourProduct" :key="index" >
            <img
            class="d-block img-fluid w-100"
            :src="item.image.url"
            alt="image"
            />
            <div class="product-title mb-1" @click="$router.push('/product')">
              {{ item.name }}
            </div>
            <div class="product-rating">
              <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= item.rating}"></i>
            </div>
            <div class="product-price">{{item.price}} &euro;</div>
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
          <VueSlickCarousel v-bind="setting" :arrows="true" :dots="false">
            <div class="user-review">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-2">
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  <div class="review-name fw-900">Martin Lawrence</div>
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-1">
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  <div class="review-name fw-900">Martin Lawrence</div>
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-1">
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  <div class="review-name fw-900">Martin Lawrence</div>
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-1">
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  <div class="review-name fw-900">Martin Lawrence</div>
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-2">
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  <div class="review-name fw-900">Martin Lawrence</div>
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-2">
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  <div class="review-name fw-900">Martin Lawrence</div>
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
          </VueSlickCarousel>
        </div>
      </b-container>
     </section>

     <!-- benefit -->
     <section class="benefit">
       <b-container>
         <b-row>
           <b-col cols="4" class="text-center">
            <img
            class="d-block img-auto img-margin"
            height="60"
            src="/shopping-bag.svg"
            alt="image"
            />
            <div class="benefit-title mt-2">
              FREE SHIPPING <br />ON ORDER + 150 &euro;
            </div>
           </b-col>
           <b-col cols="4" class="text-center">
            <img
            class="d-block img-auto img-margin"
            height="60"
            src="/shopping-bag.svg"
            alt="image"
            />
            <div class="benefit-title mt-2">
             SECURE PAYMENT <br />WITH SSL ENCRYPTION
            </div>
           </b-col>
           <b-col cols="4" class="text-center">
            <img
            class="d-block img-auto img-margin"
            height="60"
            src="/shopping-bag.svg"
            alt="image"
            />
            <div class="benefit-title mt-2">
              10 YEARS WARRANTY <br /> ON ALL ITEMS
            </div>
           </b-col>
         </b-row>
       </b-container>
     </section>

     <!-- footer -->
     <section class="footer">
       <b-container>
         <b-row>
          <b-col class="6">
            <img
            class="d-block img-auto"
            height="20"
            src="/white-logo.svg"
            alt="image"
            />
          </b-col>
          <b-col class="6">
            <b-row>
              <b-col cols="5">
                <div class="stay">STAY CONNECTED</div>
                <small>Sign up for news event offers</small>
              </b-col>
              <b-col cols="7" class="pl-1 d-flex align-items-center">
                <b-form-input
                  id="search-1"
                  class="form-subscribe"
                  type="text"
                  placeholder="enter email here"
                ></b-form-input>
                <b-link href="#" class="f-white ml-1">Subscribe</b-link>
              </b-col>
            </b-row>
            <hr class="hr-white"/>
          </b-col>
         </b-row>
         <b-row>
            <b-col cols="6">
              <p>Jalan Batu Sangian VI No.10 Kuta Utara, Bali 80361 INDONESIA <br /><br />Phone: +62 361 419 288</p>
              <div class="sosmed mt-2">
                <img
                class="d-block img-auto"
                height="24"
                src="/IG.png"
                alt="image"
                />
                <img
                class="d-block img-auto"
                height="24"
                src="/FB.png"
                alt="image"
                />
                <img
                class="d-block img-auto"
                height="24"
                src="/Youtube.png"
                alt="image"
                />
                <img
                class="d-block img-auto"
                height="24"
                src="/LinkedIn.png"
                alt="image"
                />
              </div>
            </b-col>
            <b-col cols="2">
              <div class="title-link">
                TTTM
              </div>
              <ul class="list-link">
                <li>
                  <b-link href="#">About Us</b-link>
                </li>
                <li>
                  <b-link href="#">TTTM History</b-link>
                </li>
                <li>
                  <b-link href="#">Customize &amp; Shop</b-link>
                </li>
                <li>
                  <b-link href="#">Join The Tribe</b-link>
                </li>
                <li>
                  <b-link href="#">Blog</b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="2">
              <div class="title-link">
                INFO
              </div>
              <ul class="list-link">
                <li>
                  <b-link href="#">FAQ</b-link>
                </li>
                <li>
                  <b-link href="#">Privacy Policy</b-link>
                </li>
                <li>
                  <b-link href="#">Download</b-link>
                </li>
                <li>
                  <b-link href="#">Warranty</b-link>
                </li>
                <li>
                  <b-link href="#">TTTM Affiliate Program</b-link>
                </li>
                <li>
                  <b-link @click="$router.push('/gdpr-privacy-policy')">GDPR Privacy Policy</b-link>
                </li>
              </ul>
            </b-col>
            <b-col cols="2">
              <div class="title-link">
                SERVICE
              </div>
              <ul class="list-link">
                <li>
                  <b-link href="#">My Account</b-link>
                </li>
                <li>
                  <b-link href="#">Shopping Cart</b-link>
                </li>
                <li>
                  <b-link href="#">Tracking Order</b-link>
                </li>
                <li>
                  <b-link href="#">Contact Us</b-link>
                </li>
              </ul>
            </b-col>
         </b-row>
         <b-row class="mt-2">
           <b-col cols="6">
             <div class="copyright">&copy; 2021 Ticket To The Moon. All Rights Reserved. Design &amp; Development by Hi Folks Agency</div>
           </b-col>
           <b-col cols="6">
              <img
              class="d-block img-fluid"
              src="/payment.svg"
              alt="image"
              />
           </b-col>
         </b-row>
       </b-container>
     </section>
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Alegreya+Sans:wght@300;400;500;600;900&display=swap");
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css");
</style>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import TopNavbar from'/components/top-navbar'

export default {
  name: 'MyComponent',
  components: { 
    VueSlickCarousel,
    TopNavbar
  },

  data() {
      return {
        slide: 0,
        sliding: null,
        isHidden: false,
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
        ],
        setting: {
          dots: true,
          focusOnSelect: true,
          infinite: true,
          speed: 500,
          slidesToShow: 3,
          slidesToScroll: 3,
          touchThreshold: 5,
          centerPadding: "20px"
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
