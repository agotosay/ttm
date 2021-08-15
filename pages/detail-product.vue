<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <section>
      <b-container>
        <b-row>
          <b-col cols="5" class="detail-product">
            <div class="sticky" style="position: sticky; top: 70px;">
              <img
                class="d-block img-fluid w-100 pic"
                src="/image-20.jpg"
                alt="image"
              />
              <div class="action">
                <img
                src="/upload.svg"
                alt="image"
                height="20"
                />
                <img
                src="/download.svg"
                alt="image"
                height="20"
                />
                <img
                src="/rotate.svg"
                alt="image"
                height="20"
                />
              </div>
              <div class="thumbnail">
                <img
                class="d-block img-fluid"
                src="/thumb1.png"
                alt="image"
                />
                <img
                class="d-block img-fluid"
                src="/thumb2.png"
                alt="image"
                />
                <img
                class="d-block img-fluid"
                src="/thumb3.png"
                alt="image"
                />
                <img
                class="d-block img-fluid"
                src="/thumb4.png"
                alt="image"
                />
              </div>
            </div>
          </b-col>
          <b-col cols="7" class="spec-product">
            <div class="title text-center">
              CUSTOMIZE YOUR <br />
              <span class="fw-900">travel hammock</span>
            </div>
            <!-- size -->
            <b-card class="size text-center mb-1 mt-2">
              <div class="title">SIZE</div>
              <div class="option" :class="{'active' : index === sizeSelected}" v-for="(item, index) in sizeOption" :key="index" @click="onSelectSize(index)">
                <div>{{item.name}}</div>
                <div>{{item.price}}</div>
              </div>
            </b-card>
            <!-- main color -->
            <b-card class="text-center mb-1">
              <div class="title">MAIN COLOR</div>
              <div class="color" @click="mainColor = !mainColor">
                <div class="selected-color orange"></div>
                <img
                class="ml-1 d-block"
                src="/arrow-down.svg"
                height="16"
                alt="image"
                />
              </div>
              <!-- toggle color -->
              <div class="main-color" v-if="mainColor">
                <div class="color orange"></div>
                <div class="color jade"></div>
                <div class="color old-purple"></div>
                <div class="color pink"></div>
                <div class="color green"></div>
                <div class="color blue"></div>
                <div class="color yellow"></div>
                <div class="color white"></div>
                <div class="color black"></div>
              </div>
            </b-card>
            <!-- second color -->
            <b-card class="text-center mb-1">
              <div class="title">SECOND COLOR</div>
              <div class="color" @click="secondColor = !secondColor">
                <div class="selected-color dark-brown"></div>
                <img
                class="ml-1 d-block"
                src="/arrow-down.svg"
                height="16"
                alt="image"
                />
              </div>
              <!-- toggle color -->
              <!-- toggle color -->
              <div class="main-color" v-if="secondColor">
                <div class="color dark-brown"></div>
                <div class="color jade"></div>
                <div class="color old-purple"></div>
                <div class="color pink"></div>
                <div class="color green"></div>
                <div class="color blue"></div>
                <div class="color yellow"></div>
                <div class="color white"></div>
                <div class="color black"></div>
              </div>
            </b-card>
            <!-- sleeve-->
            <b-card class="text-center mb-1">
              <div class="title">SLEEVE</div>
              <img
              class="d-block img-fluid w-100 pic"
              src="/image-26.jpg"
              alt="image"
              />
              <div class="btn w-100 d-flex align-items-center justify-content-center mt-2" @click="sleeveSelect" :class="onSleeveSelect !== 'active' ? 'btn-thirdy' : 'btn-primary'">
                SELECTED
              </div>
            </b-card>
            <!-- sleeve color -->
            <b-card class="text-center mb-1">
              <div class="title">SLEEVE COLOR</div>
              <div class="color" @click="sleeveColor = !sleeveColor">
                <div class="selected-color dark-brown"></div>
                <img
                class="ml-1 d-block"
                src="/arrow-down.svg"
                height="16"
                alt="image"
                />
              </div>
              <!-- toggle color -->
              <!-- toggle color -->
              <div class="main-color" v-if="sleeveColor">
                <div class="color dark-brown"></div>
                <div class="color jade"></div>
                <div class="color old-purple"></div>
                <div class="color pink"></div>
                <div class="color green"></div>
                <div class="color blue"></div>
                <div class="color yellow"></div>
                <div class="color white"></div>
                <div class="color black"></div>
              </div>
            </b-card>
            <!-- accessories 1 -->
            <div class="detail-title">accessories 1</div>
            <b-row>
              <b-col cols="6">
                <b-card class="text-center mb-1">
                  <div class="title">HOOK</div>
                  <img
                  class="d-block img-fluid w-100 accessories"
                  src="/image-27.png"
                  alt="image"
                  />
                  <b-button :variant="selectedAcc1 === 0 ? 'primary' : 'thirdy'" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="onSelectAcc1(0)">
                    SELECTED
                  </b-button>
                </b-card>
              </b-col>
              <b-col cols="6">
                <b-card class="text-center mb-1">
                  <div class="title">CARABINER</div>
                  <img
                  class="d-block img-fluid w-100 accessories"
                  src="/image-28.png"
                  alt="image"
                  />
                  <b-button :variant="selectedAcc1 === 1 ? 'primary' : 'thirdy'" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="onSelectAcc1(1)">
                    SELECTED
                  </b-button>
                </b-card>
              </b-col>
            </b-row>
             <!-- accessories 2 -->
            <div class="detail-title">accessories 2</div>
            <b-row>
              <b-col cols="6">
                <b-card class="text-center mb-1">
                  <div class="title">NAUTICAL ROPE</div>
                  <img
                  class="d-block img-fluid w-100 accessories"
                  src="/image-29.png"
                  alt="image"
                  />
                  <b-button :variant="selectedAcc2 === 0 ? 'primary' : 'thirdy'" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="onSelectAcc2(0)">
                    SELECTED
                  </b-button> 
                </b-card>
              </b-col>
              <b-col cols="6">
                <b-card class="text-center mb-1">
                  <div class="title">MOONSTRAP</div>
                  <img
                  class="d-block img-fluid w-100 accessories"
                  src="/image-30.png"
                  alt="image"
                  />
                  <b-button :variant="selectedAcc2=== 1 ? 'primary' : 'thirdy'" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="onSelectAcc2(1)">
                    SELECTED
                  </b-button>
                </b-card>
              </b-col>
            </b-row>
            <!-- desc accordion -->
            <div class="accordion" role="tablist">
              <div no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button block v-b-toggle.accordion-1 variant="info">
                    <img
                    class="mr-2"
                    src="/plus.png"
                    alt="image"
                    height="12"
                    />
                    Ultralight hammocks, handmade for adventures
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-1" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                  </b-card-body>
                </b-collapse>
              </div>
              <div no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button block v-b-toggle.accordion-2 variant="info">
                    <img
                    class="mr-2"
                    src="/plus.png"
                    alt="image"
                    height="12"
                    />
                    Comfort and strength are our promise
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                  </b-card-body>
                </b-collapse>
              </div>
              <div no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button block v-b-toggle.accordion-3 variant="info">
                    <img
                    class="mr-2"
                    src="/plus.png"
                    alt="image"
                    height="12"
                    />
                    easy to use
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                  </b-card-body>
                </b-collapse>
              </div>
              <div no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button block v-b-toggle.accordion-4 variant="info">
                    <img
                    class="mr-2"
                    src="/plus.png"
                    alt="image"
                    height="12"
                    />
                    specs
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                  </b-card-body>
                </b-collapse>
              </div>
              <div no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button block v-b-toggle.accordion-5 variant="info">
                    <img
                    class="mr-2"
                    src="/plus.png"
                    alt="image"
                    height="12"
                    />
                    Choose your accessories
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-5" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                  </b-card-body>
                </b-collapse>
              </div>
              <div no-body class="mb-1">
                <b-card-header header-tag="header" class="p-1" role="tab">
                  <b-button block v-b-toggle.accordion-6 variant="info">
                    <img
                    class="mr-2"
                    src="/plus.png"
                    alt="image"
                    height="12"
                    />
                    A Commitment to Global Betterment
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-6" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                  </b-card-body>
                </b-collapse>
              </div>
            </div>
            <!-- review -->
            <div class="title mt-2 text-center mb-1">REVIEW</div>
            <div class="user-review">
            <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious and comfortable, for daily use where weight is no issue, my original TTTM hammock will still be my first choice though. I am curious to test the durability over time. At this point I would be super cautious around prickly plants in order not to have it ripped. Certainly a good choice when every gram counts.</p>
            <div class="d-flex">
              <div>
                <b-avatar></b-avatar>
              </div>
              <div class="ml-2">
                <div class="review-name mb-1">Martin Lawrence</div>
                <div class="product-rating">
                  <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                </div>
                
                <div class="review-role">Moonquilt</div>
              </div>
            </div>
            </div>
            <div class="user-review">
              <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious and comfortable, for daily use where weight is no issue, my original TTTM hammock will still be my first choice though. I am curious to test the durability over time. At this point I would be super cautious around prickly plants in order not to have it ripped. Certainly a good choice when every gram counts.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-2">
                  <div class="review-name mb-1">Martin Lawrence</div>
                  <div class="product-rating">
                    <i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                  </div>
                  
                  <div class="review-role">Moonquilt</div>
                </div>
              </div>
            </div>
            <!-- leave review -->
            <b-card class="text-center mt-2">
              <div class="leave-review">
                <div class="title">tell everyone about you experience</div>
                <p>We’ll Be Grateful If You Can Let Us Know About Your Experience In Using Our Products. Please Leave Us Your Thoughts In The Form Of A Review. As Per Our System Requirement, The Review Section Is Moderated, So If You Haven’t Purchased Our Products, Your Identification Info Will Not Match Our Customer Records, And Your Review Couldn’t Be Processed.</p>
                <div class="mb-1">
                  <small class="mr-1">Your Rating</small><i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
                </div>
                <b-form-group>
                  <b-form-input
                    id="name"
                    type="text"
                    placeholder="Full name"
                    class="rounded-radius"
                  ></b-form-input>
                  <b-form-input
                    placeholder="Email"
                    type="email"
                    id="password"
                    class="mt-1 rounded-radius"></b-form-input>
                  <b-form-textarea
                    class="mt-1 rounded-radius"
                    id="textarea"
                    placeholder="Enter your review here"
                    rows="6"
                    max-rows="9"
                  ></b-form-textarea>
                  <b-button variant="primary d-block w-100 radius-corner" class="mt-1">
                    SUBMIT
                  </b-button>
                </b-form-group>
              </div>
            </b-card>
            <!-- other product -->
            <b-row class="mt-2">
              <b-col cols="6">
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
                  <b-button variant="thirdy" class="w-100 d-flex align-items-center justify-content-center mt-2 radius-corner" @click="$router.push('/detail-product')">
                    VIEW DETAIL
                    <img 
                    src="/arrow-right.svg" 
                    width="6"
                    alt="image" 
                    class="ml-1" />
                  </b-button>
                </div>
              </b-col>
              <b-col cols="6">
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
                  <b-button variant="thirdy" class="w-100 d-flex align-items-center justify-content-center mt-2 radius-corner" @click="$router.push('/detail-product')">
                    VIEW DETAIL
                    <img 
                    src="/arrow-right.svg" 
                    width="6"
                    alt="image" 
                    class="ml-1" />
                  </b-button>
                </div>
              </b-col>
            </b-row>
            <div>
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2" @click="$router.push('/detail-product')">
                VIEW ALL PRODUCTS
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
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
    Navbar,
  },

  data() {
    return {
      slide: 0,
      sliding: null,
      isHidden: false,
      sizeSelected: '',
      sizeOption: [
        {
          name: 'COMPACT (320 × 155cm / 10’5” × 4’11”)',
          price: '-10 €'
        },
        {
          name: 'COMPACT (320 × 155cm / 10’5” × 4’11”)',
          price: '-10 €'
        },
        {
          name: 'COMPACT (320 × 155cm / 10’5” × 4’11”)',
          price: '-10 €'
        }
      ],
      mainColor: false,
      secondColor: false,
      sleeveColor: false,
      onSleeveSelect: '',
      selectedAcc1: '',
      selectedAcc2: ''
    }
  },
  methods: {
    onSelectSize (index) {
      this.sizeSelected = index
    },
    sleeveSelect() {
      this.onSleeveSelect = this.onSleeveSelect === 'active' ? '' : 'active'
    },
    onSelectAcc1(index) {
      this.selectedAcc1 = index
    },
    onSelectAcc2(index) {
      this.selectedAcc2 = index
    }
  }
}
</script>