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
        <b-nav-item class="user" @click="$router.push('/signIn')">
          <img
          class="d-block img-margin"
          height="14"
          src="/user.svg"
          alt="image"
          />
        </b-nav-item>
      </b-nav>
    </div>

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
                <b-link href="#">GDPR Privacy Policy</b-link>
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
export default {
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
