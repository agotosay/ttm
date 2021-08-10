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
          Gallery
        </div>
        <VueSlickCarousel v-bind="gallerys" :arrows="true" :dots="false">
          <img
          class="img-fluid w-100"
          src="/image-31.png"
          alt="image"
          />
          <img
          class="img-fluid w-100"
          src="/image-31.png"
          alt="image"
          />
          <img
          class="img-fluid w-100"
          src="/image-31.png"
          alt="image"
          />
        </VueSlickCarousel>
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
        }
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
