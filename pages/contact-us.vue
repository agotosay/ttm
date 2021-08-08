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
    <section>
      <b-container>
        <div class="title mb-2">Send a message</div>
        <b-row>
          <b-col cols="4">
            <b-form-group>
              <b-form-input
                id="name"
                type="text"
                placeholder="First name"
                class="mb-1 rounded-radius"
              ></b-form-input>
              <b-form-input
                id="name"
                type="text"
                placeholder="Last name"
                class="mb-1 rounded-radius"
              ></b-form-input>
              <b-form-select v-model="selected" :options="options" class="mb-1 rounded-radius"></b-form-select>
              <b-form-textarea
                class="mb-1 rounded-radius"
                id="textarea"
                v-model="text"
                placeholder="Your message"
                rows="6"
                max-rows="9"
              ></b-form-textarea>
              <div class='file mb-1'>
                <label for='input-file'>
                  <span class="material-icons">Upload attachment</span>
                </label>
                <input id='input-file' type='file' />
              </div>
              <b-form-checkbox
                id="checkbox-1"
                v-model="status"
                name="checkbox-1"
                value="accepted"
                unchecked-value="not_accepted"
              >
                By Checking This, You Agree With Out <b-link class="text-blue">GDPR Privacy Policy</b-link>
              </b-form-checkbox>
              <b-button variant="primary d-block w-100" class="mt-1">
                SUBMIT
              </b-button>
            </b-form-group>
          </b-col>
          <b-col cols="1"></b-col>
          <b-col cols="7">
            <div class="info-contact">
              <div class="title text-yellow mb-2">GET IN TOUCH</div>
              <p>Jalan Batu Sangian VI No.10 Kuta Utara, Bali 80361 INDONESIA</p>
              <p>Phone: +62 361 419 288</p>
              <div class="sosmed mt-2 d-flex align-items-center">
                <img
                class="d-block img-auto mr-1"
                height="24"
                src="/instagram.svg"
                alt="image"
                />
                <img
                class="d-block img-auto mr-1"
                height="24"
                src="/facebook.svg"
                alt="image"
                />
                <img
                class="d-block img-auto mr-1"
                height="24"
                src="/youtube.svg"
                alt="image"
                />
                <img
                class="d-block img-auto mr-1"
                height="24"
                src="/linkedin.svg"
                alt="image"
                />
              </div>
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
        gallerys: {
          centerMode: true,
          centerPadding: '60px',
          slidesToShow: 1,
          arrows: true,
        },
        selected: null,
        options: [
          { value: null, text: 'Please select a subject' },
          { value: 'a', text: 'Option A' },
          { value: 'b', text: 'Option B' },
          { value: 'c', text: 'Option C' },
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
