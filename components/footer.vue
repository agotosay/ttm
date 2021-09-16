<template>
  <section class="footer">
    <b-container>
      <b-row>
      <b-col cols="12" lg="5">
        <img
        class="d-block img-auto img-logo-footer"
        height="20"
        src="/white-logo.svg"
        alt="image"
        />
      </b-col>
      <b-col cols="12" lg="7">
        <b-row>
          <b-col cols="6" lg="5">
            <img
            class="d-block img-fluid img-stay"
            src="/stay-connected.svg"
            alt="image"
            />
          </b-col>
          <b-col cols="12" lg="7" class="pl-1 d-flex align-items-center">
            <b-form-input
              id="search-1"
              class="form-subscribe"
              type="text"
              placeholder="enter email here"
            ></b-form-input>
            <b-button variant="primary" class="rounded-radius ml-1 btn-subsc">SUBSCRIBE</b-button>
          </b-col>
        </b-row>
      </b-col>
      </b-row>
      <b-row class="mt-2">
        <b-col cols="12" lg="5">
          <p>Jalan Batu Sangian VI No.10 Kuta Utara,<br /> Bali 80361 INDONESIA <br /><br />Phone: +62 361 419 288</p>
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
        <b-col cols="4" lg="2">
          <div class="title-link">
            TTTM
          </div>
          <ul class="list-link">
            <li>
              <b-link @click="$router.push('/about-us')">About Us</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/ttm-history')">TTTM History</b-link>
            </li>
            <li>
              <b-link>Customize &amp; Shop</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/join-tribe')">Join The Tribe</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/foundation')">TTTM Foundation</b-link>
            </li>
          </ul>
        </b-col>
        <b-col cols="4" lg="2">
          <div class="title-link">
            INFO
          </div>
          <ul class="list-link">
            <li>
              <b-link @click="$router.push('/faq')">FAQ</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/privacy-policy')">Privacy Policy</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/download')">Download</b-link>
            </li>
            <li>
              <b-link  @click="$router.push('/warranty')">Warranty</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/affiliate')">TTTM Affiliate Program</b-link>
            </li>
            <li>
              <b-link  @click="$router.push('/gdpr-privacy-policy')">GDPR Privacy Policy</b-link>
            </li>
          </ul>
        </b-col>
        <b-col cols="4" lg="2">
          <div class="title-link">
            SERVICE
          </div>
          <ul class="list-link">
            <li>
              <b-link href="#">My Account</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/shopping-cart')">Shopping Cart</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/tracking-order')">Tracking Order</b-link>
            </li>
            <li>
              <b-link @click="$router.push('/contact-us')">Contact Us</b-link>
            </li>
          </ul>
        </b-col>
      </b-row>
      <b-row class="mt-2">
        <b-col cols="12" lg="6">
          <div class="copyright">&copy; 2021 Ticket To The Moon. All Rights Reserved. Design &amp; Development by Hi Folks Agency</div>
        </b-col>
        <b-col cols="12" lg="6">
          <img
          class="d-block img-fluid img-payment"
          src="/payment.svg"
          alt="image"
          />
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>