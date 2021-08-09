<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

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
