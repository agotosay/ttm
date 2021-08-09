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
        <div class="title mb-2">Warranty policy</div>
        <p>Ticket to the Moon products carry a 10 years warranty against defects in workmanship and materials. Defective or damaged products should be returned to us for evaluation and will be repaired or replaced at our discretion. We ensure that all our products are leaving our factory in good condition and free from manufacturing defects.Warranty issues are settled by replacement or exchange, no credits or refunds.</p>
        <p>We recommend you register at www.ticketothemoon.com/register to give your hammock the ensured 10 years warranty without using your bill or receipt.</p>
        <p>If you purchased your TTTM product through a shop, you may try first to contact the retailer with a proof of purchase and a detailed information about the faults of your product.</p>
        <p>Each warranty item is processed individually. Ticket to the Moon recommends to get in contact with us before you send your hammock by mail. Please allow 2-3 business days for response once the application is submitted.</p>
        <p>Nylon fabric is extremely resistant but also fragile…Smaller holes (up to 5cm) or burns can be repaired with a repair patch. The good news is that we will never let our users down so it is available for shipping from the factory, please contact us for further info. FYI nylon repair patch or nylon repair tape can also be sourced locally!</p>
        <p>PLEASE NOTE This warranty only covers manufacturing defects and does not cover:</p>
        <p>UV Damage (discoloration and brittleness causes tearing)</p>
        <p>Elemental/Accidental Damage (wind, burns, animal bites)</p>
        <p>Improper care or use (hanging over 45 cm / 18″, use of sharp objects,</p>
        <p>exceeding the weight capacity of 200kg / 440 lbs, jumping, excessive swinging)</p>
        <p>Normal wear and tear</p>
        <p>For more information about keeping your gear in good condition, please visit our FAQs Page</p>
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
