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
        TRACKING ORDER
      </div>
      <p>To track your order please select your Couriers and enter your Tracking Code in the box and press the "Track Order" button. You can find your Tracking Code and Couriers in the shipping confirmation email that was emailed to you.</p>
      <b-row class="tracking-order">
        <b-col cols="12" lg="9" offset="1">
          <div class="d-flex align-items-center justify-content-center wrapper-tracking">
            <div class="w-100">
              <b-form class="mb-1 tracking-input">
                <label>Expedition :</label>
                <b-form-input type="number" id="for-phone" placeholder="" class="rounded-radius"/>
              </b-form>
              <b-form class="mb-1 tracking-input">
                <label>Tracking Code :</label>
                <b-form-input type="number" id="for-phone" placeholder="" class="rounded-radius"/>
              </b-form>
            </div>
            <b-button variant="primary" class="btn-tracking">
              TRACK ORDER
              <img 
                src="/arrow-right.svg" 
                width="6"
                alt="image" 
                class="ml-1" />
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
      isHidden: false,
    }
  }
}
</script>
