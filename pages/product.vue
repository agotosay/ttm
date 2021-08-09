<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- product -->
    <section>
      <div class="box-product">
        <b-row>
          <b-col cols="3" class="left">
            <div class="title">TRAVEL HAMMOCK</div>
            <div class="add-sleeve">
              <div class="title">SLEEVE</div>
              <p>Cover Your Hammock While Not In Use!</p>
              <b-button variant="primary d-block" class="mt-1">
                ADD
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
          <b-col cols="6">
            <img
              class="d-block img-fluid img-margin img-product"
              src="/img-product.png"
              alt="image"
            />
          </b-col>
          <b-col cols="3">
            <div class="box-price">
              asd
              <b-button variant="primary d-block w-100" class="mt-2">
                ADD TO CART
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </div>
          </b-col>
        </b-row>
      </div>
    </section>

    <!-- option -->
    <b-tabs content-class="mt-3 tab-padding" align="center">
      <b-tab title="Size" active>
        <div class="fw-900 text-center mb-2">320 x 200 cm / 10’5” x 6’6”</div>
        <b-container>
          <b-row class="size-info">
            <b-col cols="2">
              <img
              class="d-block img-margin img-size"
              src="/img-3.png"
              alt="image"
              />
              <div class="info-desc">Mini</div>
              <div class="info-price">59.95 &euro;</div>
              <b-button variant="primary d-block img-margin" class="mt-2">
                ADD
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </b-col>
            <b-col cols="2">
              <img
              class="d-block img-margin img-size"
              src="/img-3.png"
              alt="image"
              />
              <div class="info-desc">Mini</div>
              <div class="info-price">59.95 &euro;</div>
              <b-button variant="primary d-block img-margin" class="mt-2">
                ADD
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </b-col>
            <b-col cols="2">
              <img
              class="d-block img-margin img-size"
              src="/img-3.png"
              alt="image"
              />
              <div class="info-desc">Mini</div>
              <div class="info-price">59.95 &euro;</div>
              <b-button variant="primary d-block img-margin" class="mt-2">
                ADD
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </b-col>
            <b-col cols="2">
              <img
              class="d-block img-margin img-size"
              src="/img-3.png"
              alt="image"
              />
              <div class="info-desc">Mini</div>
              <div class="info-price">59.95 &euro;</div>
              <b-button variant="primary d-block img-margin" class="mt-2">
                ADD
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </b-col>
            <b-col cols="2">
              <img
              class="d-block img-margin img-size"
              src="/img-3.png"
              alt="image"
              />
              <div class="info-desc">Mini</div>
              <div class="info-price">59.95 &euro;</div>
              <b-button variant="primary d-block img-margin" class="mt-2">
                ADD
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </b-col>
            <b-col cols="2">
              <img
              class="d-block img-margin img-size"
              src="/img-3.png"
              alt="image"
              />
              <div class="info-desc">Mini</div>
              <div class="info-price">59.95 &euro;</div>
              <b-button variant="primary d-block img-margin" class="mt-2">
                ADD
                <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
              </b-button>
            </b-col>
          </b-row>
        </b-container>
      </b-tab>
      <b-tab title="Color"><p>Color</p></b-tab>
      <b-tab title="Accessories"><p>Accessories</p></b-tab>
    </b-tabs>
    
    <!-- find store -->
    <div class="find-store">
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
    </div>

    <!-- list -->
    <section class="listing-product">
      <b-container>
        <b-row>
          <b-col cols="6" offset-md="3">
            <ul>
              <li>TRAVEL HAMMOCK</li>
              <li>Comfort and strength are our promise</li>
              <li>Ease of use</li>
              <li>Choose your size and color</li>
              <li>Choose your accessories</li>
              <li>A Commitment to Global Betterment</li>
            </ul>
          </b-col>
        </b-row>
      </b-container>
    </section>

    <hr />

    <!-- newest review -->
    <section>
      <b-container>
        <div class="title mb-2">NEWEST REVIEW</div>
        <b-row class="pl-1 pr-1">
          <b-col cols="6">
            <b-row class="newest-review">
              <b-col cols="5" class="pl-0 pr-0">
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
              </b-col>
              <b-col cols="7" class="pl-0 pr-0">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
              </b-col>
            </b-row>
            <b-row class="newest-review">
              <b-col cols="5" class="pl-0 pr-0">
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
              </b-col>
              <b-col cols="7" class="pl-0 pr-0">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
              </b-col>
            </b-row>
            <b-row class="newest-review">
              <b-col cols="5" class="pl-0 pr-0">
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
              </b-col>
              <b-col cols="7" class="pl-0 pr-0">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.</p>
              </b-col>
            </b-row>
          </b-col>
          <b-col cols="6" class="leave-review">
            <div class="title">Be The First To Review on this product</div>
            <div class="mb-1">
              <small class="mr-1">Your Rating</small><i class="fas fa-star" v-for="indexRating in 5" :key="indexRating" :class="{'text-warning': indexRating <= 5}"></i>
            </div>
            <b-form-group>
              <b-form-input
                id="name"
                type="text"
                placeholder="Name"
              ></b-form-input>
              <b-form-input
                placeholder="Email"
                type="email"
                id="password"
                class="mt-1"></b-form-input>
              <b-form-textarea
                class="mt-1"
                id="textarea"
                v-model="text"
                placeholder="Enter your review here"
                rows="6"
                max-rows="9"
              ></b-form-textarea>
              <b-button variant="primary d-block" class="mt-1">
                SUBMIT
              </b-button>
            </b-form-group>
          </b-col>
        </b-row>
      </b-container>
    </section>

    <!-- products -->
    <section class="our-product">
      <b-container>
        <div class="title text-center">
          RELATED PRODUCTS
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
import TopNavbar from'/components/top-navbar'
import Footer from'/components/footer'
import Navbar from'/components/navbar'

export default {
  name: 'MyComponent',
  components: { 
    TopNavbar,
    Footer,
    Navbar
  },

  data() {
    return {
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
    }
  }
}
</script>
