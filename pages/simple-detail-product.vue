<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- desc product -->
    <section class="position-relative">
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
              moonstraps
            </div>
            <div class="product-price">27.95<span>&euro;</span></div>
            <div class="text-center mt-1">
              <b-button variant="primary" class="d-flex align-items-center justify-content-center img-margin" @click="modalShow = !modalShow">
                ADD TO CART 
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
            <!-- main color -->
            <b-card class="text-center mb-1 mt-3">
              <p>Ticket to the Moon´s Moon Straps, the daisy-chain suspension solution that combines tree-friendly properties, small packing size, higher durability and higher load.</p>
            </b-card>
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
                    The most flexible suspension solution: reliable under all circumstances
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-1" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Moon Straps can individually support loads up to 300kg, making them reliable tools in demanding situations. They’re excellent compliments to all sizes of hammocks in order to accommodate multiple users. Each strap is highly durable and keeps the bark of the tree safe. The textured strap is even compatible with smoother surfaces, such as metallic poles. 
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
                   SPECS
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    <b-row>
                      <b-col cols="6">
                        Dimensions: 
                      </b-col>
                      <b-col cols="6">2cm x 260cm x 2cm (0.8in x 8.5ft x 0.8in)</b-col>
                    </b-row>
                    <b-row>
                      <b-col cols="6">
                        Maximum static load:
                      </b-col>
                      <b-col cols="6">300kg (660lbs)</b-col>
                    </b-row>
                    <b-row>
                      <b-col cols="6">
                        Net weight:
                      </b-col>
                      <b-col cols="6">216g (7.6oz)</b-col>
                    </b-row>
                    <b-row>
                      <b-col cols="6">
                        Material:
                      </b-col>
                      <b-col cols="6">100% polyester</b-col>
                    </b-row>
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
                    Includes
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    <p>2 × MOONSTRAPS </p>
                    <p>Handy carruing poch</p>
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
                    Features
                  </b-button>
                </b-card-header>
                <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
                  <b-card-body>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                  </b-card-body>
                </b-collapse>
              </div>
            </div>
          </b-col>
        </b-row>
      </b-container>
      <div class="badge-fast for-product">
        <b-link href="">10-year <br>warranty</b-link>  
      </div>
    </section>

    <!-- review -->
    <section class="reviews">
      <b-container>
        <div class="title text-center mb-2">
          REVIEWS
        </div>
        <div>
          <VueSlickCarousel v-bind="reviews" :arrows="true" :dots="true">
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
              <p>I was blown away by the tiny packing size and the very thin and light material. It certainly is the lightest hammock I have ever come across. The material feels like very fine silk, thin as glad wrap. However, it does not feel sweaty and does not seem to be noisy. For its minimalistic design it is very spacious.</p>
              <div class="d-flex">
                <div>
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-1">
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
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-1">
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
                  <b-avatar></b-avatar>
                </div>
                <div class="ml-1">
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

    <!-- leave review -->
    <section>
      <b-container>
        <b-card class="card-pad">
          <div class="leave-review">
            <b-row>
              <b-col cols="6">
                <div class="title mb-1">tell everyone about you experience</div>
                <p>We’ll Be Grateful If You Can Let Us Know About Your Experience In Using Our Products. Please Leave Us Your Thoughts In The Form Of A Review. As Per Our System Requirement, The Review Section Is Moderated, So If You Haven’t Purchased Our Products, Your Identification Info Will Not Match Our Customer Records, And Your Review Couldn’t Be Processed.</p>
              </b-col>
              <b-col cols="6">
                <div class="mb-1">
                  <small class="mr-1">Your Rate</small><i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
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
              </b-col>
            </b-row>
          </div>
        </b-card>
      </b-container>
    </section>

    <!-- other product -->
    <b-container>
      <div class="title text-center mb-2">
        Related Products
      </div>
      <b-row class="mt-2">
        <b-col cols="3">
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
        <b-col cols="3">
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
        <b-col cols="3">
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
        <b-col cols="3">
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
      <div class="text-center">
        <b-button variant="primary" class="mt-2 mb-3" @click="$router.push('/detail-product')">
          VIEW ALL PRODUCTS
          <img 
          src="/arrow-right.svg" 
          width="6"
          alt="image" 
          class="ml-1" />
        </b-button>
      </div>
    </b-container>

    <!-- modal add to cart -->
    <b-modal id="modal-center" hide-footer centered title="ADDED TO CART" v-model="modalShow" size="xl">
      <hr>
      <div class="modal-cart d-flex align-items-center justify-between">
        <div class="pic">
          <img
          class="d-block"
          src="/image-41.jpg"
          alt="image"
          />
        </div>
        <div class="desc ml-1">
          <span class="fw-500">TRAVEL HAMMOCK Size: </span> Compact - 320x155cm / 10’5”x4’11” Compact - 320x155cm / 10’5”x4’11” 
        </div>
        <b-button variant="primary" class="d-flex align-items-center justify-content-center radius-corner" @click="$router.push('/detail-product')">
          SEE THE CART
          <img 
          src="/arrow-right.svg" 
          width="6"
          alt="image" 
          class="ml-1" />
        </b-button>
      </div>
      <hr>
      <b-row class="mt-2">
        <b-col cols="3">
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
            <b-button variant="thirdy" class="w-100 d-flex align-items-center justify-content-center mt-1 radius-corner" @click="$router.push('/detail-product')">
              VIEW DETAIL
              <img 
              src="/arrow-right.svg" 
              width="6"
              alt="image" 
              class="ml-1" />
            </b-button>
          </div>
        </b-col>
        <b-col cols="3">
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
            <b-button variant="thirdy" class="w-100 d-flex align-items-center justify-content-center mt-1 radius-corner" @click="$router.push('/detail-product')">
              VIEW DETAIL
              <img 
              src="/arrow-right.svg" 
              width="6"
              alt="image" 
              class="ml-1" />
            </b-button>
          </div>
        </b-col>
        <b-col cols="3">
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
            <b-button variant="thirdy" class="w-100 d-flex align-items-center justify-content-center mt-1 radius-corner" @click="$router.push('/detail-product')">
              VIEW DETAIL
              <img 
              src="/arrow-right.svg" 
              width="6"
              alt="image" 
              class="ml-1" />
            </b-button>
          </div>
        </b-col>
        <b-col cols="3">
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
            <b-button variant="thirdy" class="w-100 d-flex align-items-center justify-content-center mt-1 radius-corner" @click="$router.push('/detail-product')">
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
      <div class="text-center">
        <b-button variant="primary" class="mt-3 mb-1 radius-corner">
          VIEW ALL PRODUCTS
          <img 
          src="/arrow-right.svg" 
          width="6"
          alt="image" 
          class="ml-1" />
        </b-button>
      </div>
    </b-modal>

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
      selectedAcc2: '',
      reviews: {
        centerMode: true,
        centerPadding: '60px',
        slidesToShow: 2,
        arrows: true,
      },
      modalShow: false
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