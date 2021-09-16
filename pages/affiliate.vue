<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

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
          <b-col cols="12" lg="6">
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
              <b-col cols="12" lg="3">
                <b-form class="mb-1">
                  <label>Age :</label>
                  <b-form-input type="number" id="for-phone" placeholder="Age" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="12" lg="5">
                <b-form class="mb-1">
                  <label>Nationality :</label>
                  <b-form-input type="number" id="for-phone" placeholder="Nationality" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="12" lg="4">
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
          <b-col cols="12" lg="6">
            <div class="fw-600 mb-2">Occupation / Field of Interest :</div>
            <b-form-group class="d-flex justify-content-between mobile">
              <label>Occupation / Field of Interest :</label>
              <div class="d-flex w-100 mt-0h mobile">
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
                placeholder="Tell us why we should choose you as our ambassador ?"
                rows="6"
                max-rows="9"
            ></b-form-textarea>
            </b-form>
            <b-form-checkbox
              id="checkbox-1"
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
