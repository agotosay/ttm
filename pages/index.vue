<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- carousel -->
    <div class="position-relative">
      <b-carousel
        id="carousel-1"
        v-model="slide"
        :interval="4000"
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

    <!-- img separator -->
    <section>
      <b-container>
        <div class="img-separator with-info position-relative">
          <div class="info right bc-yellow">
            <div class="title">TRAVEL <br />HAMMOCKS</div>
            <p class="mb-1">I was blown away by the tiny packing size and the very thin and light material. It certainly lightest hammock I have ever come across.</p>
            <b-button variant="secondary" class="mt-1 w-100">
              SEE ALL HAMMOCKS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </div>
          <img
            class="d-block w-100 img-margin"
            height="600"
            src="/banner2.jpg"
            alt="image"
          />
        </div>
      </b-container>
    </section>

    <!-- products -->
    <section class="our-product">
      <b-container>
        <div class="title text-center">
          OUR PRODUCTS
        </div>
        <VueSlickCarousel v-bind="products" :arrows="false" :dots="true">
          <div class="our-products pointer" v-for="(item, index) in ourProduct" :key="index"  @click="$router.push('/all-product')">
            <img
            class="d-block img-fluid w-100 img-card-product"
            :src="item.image.url"
            alt="image"
            />
            <div class="product-title mb-1">
              {{ item.name }}
            </div>
            <div class="product-rating">
              <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= item.rating}"></i>
            </div>
            <div class="product-price">{{item.price}} &euro;</div>
            <b-button variant="thirdy" class="w-100 d-flex align-items-center justify-content-center mt-2">
            VIEW DETAILS
            </b-button>
          </div>
        </VueSlickCarousel>
        <div class="text-center mt-2">
          <b-button variant="primary" class="mt-2" @click="$router.push('/all-product')">
          VIEW ALL PRODUCTS
          <img 
            src="/arrow-right.svg" 
            width="6"
            alt="image" 
            class="ml-1" />
          </b-button>
        </div>
      </b-container>
    </section>

    <!-- img separator -->
    <section>
      <b-container>
        <div class="img-separator with-info position-relative">
          <div class="info left bc-blue">
            <div class="title">MORE THAN <br />HAMMOCKS</div>
            <p class="mb-1 text-center">Building better living for the people through</p>
            <p class="fw-500 text-center">TTTM FOUNDATION</p>
            <b-button variant="secondary" class="mt-1 w-100">
              SEE ALL PRODUCTS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
            </b-button>
          </div>
          <img
            class="d-block w-100 img-margin"
            height="600"
            src="/banner3.jpg"
            alt="image"
          />
        </div>
      </b-container>
    </section>

    <!-- benefit -->
    <section>
      <b-container class="benefit">
        <b-row>
          <b-col cols="4" class="text-center">
          <img
          class="d-block img-auto img-margin"
          height="60"
          src="/Frame1.svg"
          alt="image"
          />
          <div class="benefit-title mt-2">
            10 YEARS WARRANTY
          </div>
          <div class="benefit-subtitle">ON ALL ITEMS</div>
          </b-col>
          <b-col cols="4" class="text-center">
          <img
          class="d-block img-auto img-margin"
          height="60"
          src="/Frame2.svg"
          alt="image"
          />
            <div class="benefit-title mt-2">
            SECURE PAYMENT
          </div>
          <div class="benefit-subtitle">WITH SSL ENCRYPTION</div>
          </b-col>
          <b-col cols="4" class="text-center">
          <img
          class="d-block img-auto img-margin"
          height="60"
          src="Frame3.svg"
          alt="image"
          />
          <div class="benefit-title mt-2">
            FREE SHIPPING
          </div>
          <div class="benefit-subtitle">ON ORDER +150 &euro;</div>
          </b-col>
        </b-row>
      </b-container>
    </section>

    <!-- review -->
    <section class="reviews">
      <b-container>
        <div class="title text-center">
          REVIEWS
        </div>
        <div>
          <VueSlickCarousel v-bind="reviews" :arrows="true" :dots="false">
            <div class="user-review">
              <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious and comfortable, for daily use where weight is no issue, my original TTTM hammock will still be my first choice though. I am curious to test the durability over time. At this point I would be super cautious around prickly plants in order not to have it ripped. Certainly a good choice when every gram counts.</p>
              <div class="d-flex">
                <div>
                  <div class="review-name mb-1">Martin Lawrence</div>
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious.</p>
              <div class="d-flex">
                <div>
                  <div class="review-name mb-1">Martin Lawrence</div>
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious. I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap.</p>
              <div class="d-flex">
                <div>
                  <div class="review-name mb-1">Martin Lawrence</div>
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <div class="user-review">
              <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious and comfortable, for daily use where weight is no issue, my original TTTM hammock will still be my first choice though. I am curious to test the durability over time. At this point I would be super cautious around prickly plants in order not to have it ripped. Certainly a good choice when every gram counts. I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious and comfortable.</p>
              <div class="d-flex">
                <div>
                  <div class="review-name mb-1">Martin Lawrence</div>
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
          </VueSlickCarousel>
        </div>
      </b-container>
    </section>

    <!-- others -->
    <section>
      <b-container>
        <b-row>
          <b-col cols="6" class="pr-0">
            <div class="join-tribe">
              <div class="title">
                JOIN THE <br />
                #TTTM <br />
                TRIBE
              </div>
              <p>Post your stories with #TTTM hashtag to be featured <br />on our official Instagram page. </p>
              <b-button variant="secondary" class="mt-1 w-100">
              SEE ALL HAMMOCKS
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
            <img
            class="d-block img-fluid w-100 img-tribe"
            src="/image-17.png"
            alt="image"
            /> 
          </b-col>
          <b-col cols="6" class="pl-0">
            <div class="d-flex">
              <img
              class="d-block img-fluid w-100"
              src="/image-12.png"
              alt="image"
              />  
              <img
              class="d-block img-fluid w-100"
              src="/image-13.png"
              alt="image"
              />  
            </div>
            <div>
              <img
              class="d-block img-fluid w-100"
              src="/image-14.png"
              alt="image"
              />  
            </div>
            <div class="d-flex">
              <img
              class="d-block img-fluid w-100"
              src="/image-15.png"
              alt="image"
              />  
              <img
              class="d-block img-fluid w-100"
              src="/image-16.png"
              alt="image"
              />  
            </div>
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
        },
        products: {
          centerMode: true,
          centerPadding: '60px',
          slidesToShow: 3,
          autoplay: false,
        },
        reviews: {
          centerMode: true,
          centerPadding: '60px',
          slidesToShow: 2,
          arrows: true,
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
