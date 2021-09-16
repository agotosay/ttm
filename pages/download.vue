<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
   <section>
      <b-container class="gallery">
        <div class="title text-center mb-2">
          DOWNLOAD
        </div>
        <b-row>
          <b-col cols="12" lg="6" class="mb-2">
            <div class="download">
              <img
              class="d-block img-fluid w-100"
              src="/image-2.jpg"
              alt="image"
              />
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2">
                B2B Catalogue 2021
              </b-button>
            </div>
          </b-col>
          <b-col cols="12" lg="6" class="mb-2">
            <div class="download">
              <img
              class="d-block img-fluid w-100"
              src="/image-3.jpg"
              alt="image"
              />
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2">
                Guideline Book
              </b-button>
            </div>
          </b-col>
          <b-col cols="12" lg="6" class="mb-2">
            <div class="download">
              <img
              class="d-block img-fluid w-100"
              src="/image-4.jpg"
              alt="image"
              />
              <b-button variant="primary" class="w-100 d-flex align-items-center justify-content-center mt-2">
                Ticket To The Moon Foundation
              </b-button>
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
        slide: 0,
        sliding: null,
        isHidden: false,
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
