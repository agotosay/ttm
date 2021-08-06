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
      class="d-block img-fluid w-100"
      height="300"
      src="/img-3.png"
      alt="image"
      />
      <b-container class="box-desc">
        <div class="title mb-2">GDPR PRIVAY POLICY</div>
        <div class="subtitle mb-1">DEFINITIONS</div>
        <ul class="pl-1 definitions">
          <li>
            TICKET TO THE MOON Trademark<br />
            PT. Ayunan Bulan International<br />
            Jalan Batu Sangian VI No.10, 80361 Bali, Indonesia
          </li>
          <li>
            GDPR<br />
            General Data Protection Regulation Act.
          </li>
          <li>
            Data Controller<br />
            Data controller means the natural or legal person who(oether alone or jointhly or in common with other persons) determines the purposes for which and the manner in which any personal information are, or are to be, processed.
          </li>
          <li>
            Data Processor<br />
            Data Processor means any natural or legal person who processes the data on behalf of the Data Controller.
          </li>
          <li>
            Data Subject<br/>
            Data Subject is any living individual who is using our Service and is the subject of Personal Data.
          </li>
        </ul>
        <div class="mt-3">
          <b-row>
            <b-col cols="6">
              <ul class="pl-1 left-tab">
                <li @click="asd">Principles for processing personal data</li>
                <li>What personal data we collcet and process</li>
                <li>How we use the personal data</li>
                <li>Legal basis for collecting and processing personal data</li>
                <li>Retention of personal data</li>
              </ul>
            </b-col>
            <b-col cols="6">
              <div class="fw-500 mb-1">Our priciples for processing personal data are:</div>
              <ul class="pl-1">
                <li>Fairness and lawfulness.</li>
                <li>When we process personal data, the individual rights of the Data Subjects must be protected.</li>
                <li>All personal data must be collected and processed in a legal and fair manner.<br /> Restricted to a specific purpose.</li>
                <li>The Personal data of Data Subject must be processed only for specific purposes.<br /> Transparency.</li>
                <li>The Data Subject must be informed of how his/her data is being collected, processed and used.</li>
              </ul>
            </b-col>
          </b-row>
        </div>
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
