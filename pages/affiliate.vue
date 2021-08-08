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
      <img
      class="d-block w-100 img-auto"
      height="300"
      src="/img-3.png"
      alt="image"
      />
      <b-container class="box-desc">
        <div class="title mb-2">TTTM AFFILIATE PROGRAM</div>
        <p>Interested in becoming one of our ambassadors and represent the Tribe?</p>
        <p>If you are a traveler, blogger, social media influencer or adventurer who likes to connect with people and share your outdoor adventures, bring your TICKETTOTHEMOON product and your enthusiasm: you may be the right person to be part of the TICKETTOTHEMOON affiliate program.</p>
        <p>By being a TICKETTOTHEMOON ambassador, you will receive a promotional code that you can share. Customers who buy on our website with your code will get 10% off their order! What about you? As soon as the total amount of orders made with your code exceeds 250€, you have the choice: Spend the amount earned on our website or receive a bank transfer from us. If you use this amount to purchase new TICKETTOTHEMOON products on our site, your amount to be spent will be equal to 20% of the total purchase of your community. If you choose the bank transfer, it will be equal to 10% of the total purchases. </p>
        <p>Become an ambassador by filling out the form below: why are you the ideal person, the one we are looking for? Qualified candidates will be contacted by members of our tribe and you will have the privilege of receiving a discount code that you can pass on to your followers. It will allow you to increase your rewards as people use it.</p>
        <b-row class="mt-2">
          <b-col cols="6">
            <div class="fw-600 mb-2">PERSONAL DETAILS :</div>
            <b-form class="mb-1">
              <label>First name :</label>
              <b-form-input type="text" id="first-name" placeholder="First name" class="rounded-radius"/>
            </b-form>
            <b-form class="mb-1">
              <label>Last name :</label>
              <b-form-input type="text" id="last-name" placeholder="Last name" class="rounded-radius"/>
            </b-form>
            <b-form class="mb-1">
              <label>Email :</label>
              <b-form-input type="email" id="for-email" placeholder="Email" class="rounded-radius"/>
            </b-form>
            <b-form class="mb-1">
              <label>Phone :</label>
              <b-form-input type="text" id="for-phone" placeholder="Phone" class="rounded-radius"/>
            </b-form>
            <b-row>
              <b-col cols="3">
                <b-form class="mb-1">
                  <label>Age :</label>
                  <b-form-input type="number" id="for-phone" placeholder="Age" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="5">
                <b-form class="mb-1">
                  <label>Nationality :</label>
                  <b-form-input type="number" id="for-phone" placeholder="Nationality" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="4">
                <b-form-group class="d-flex justify-content-between">
                  <label>Sex :</label>
                  <div class="d-flex w-100 mt-0h">
                    <b-form-radio name="some-radios" value="A" class="mr-1">Male</b-form-radio>
                    <b-form-radio name="some-radios" value="B">Female</b-form-radio>
                  </div>
                </b-form-group>
              </b-col>
            </b-row>
          </b-col>
          <b-col cols="6">
            <div class="fw-600 mb-2">Occupation / Field of Interest :</div>
            <b-form-group class="d-flex justify-content-between">
              <label>Occupation / Field of Interest :</label>
              <div class="d-flex w-100 mt-0h">
                <b-form-radio name="some-radios" value="A" class="mr-1">Blogger</b-form-radio>
                <b-form-radio name="some-radios" value="B" class="mr-1">Influencer</b-form-radio>
                <b-form-radio name="some-radios" value="C" class="mr-1">Traveller</b-form-radio>
                <b-form-radio name="some-radios" value="D" class="mr-1">Adventurer</b-form-radio>
              </div>
            </b-form-group>
            <b-form class="mb-1">
              <label>Personal Description :</label>
              <b-form-textarea
                id="textarea"
                v-model="text"
                placeholder="Tell us why we should choose you as our ambassador ?"
                rows="6"
                max-rows="9"
            ></b-form-textarea>
            </b-form>
            <b-form-checkbox
              id="checkbox-1"
              v-model="status"
              name="checkbox-1"
              value="accepted"
              unchecked-value="not_accepted"
            >
              By Checking This, You Agree With Out <b-link class="text-blue">GDPR Privacy Policy</b-link>
            </b-form-checkbox>
            <b-button variant="primary d-block" class="mt-1">
              SUBMIT
            </b-button>
          </b-col>
        </b-row>
      </b-container>
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
