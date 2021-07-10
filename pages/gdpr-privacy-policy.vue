<template>
  <div class="position-relative">
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

    <!-- img -->
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
      
    }
  }
}
</script>
