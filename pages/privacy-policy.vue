<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
    <div class="static-info">
      <div class="position-relative">
        <img
        class="d-block w-100 img-auto"
        height="500"
        src="/image 40.jpg"
        alt="image"
        />
      </div>
    </div>

    <section class="pad-side">
      <div class="d-flex align-items-center justify-content-between">
        <div class="title">Privacy Policy</div>
      </div>
      <b-row class="mt-2">
        <b-col cols="5">
          <div class="faq-category mt-2">
            <div class="category active">INFORMATION COLLECTION</div>
            <div class="category">INFORMATION PROTECTION</div>
            <div class="category">COOKIES</div>
            <div class="category">INFORMATION DISCLOSURE TO OUTSIDE PARTIES</div>
          </div>
        </b-col>
        <b-col cols="7">
          <!-- desc accordion -->
          <div class="accordion faq" id="menu-kategori1">
            <p>We (PT. Ayunan Bulan International) collect information when you register on our website. We ask for your name, email address and shipping/billing information. You may, however, visit our website anonymously.</p>
            <p>The information we collect from you may be used:</p>
            <ul class="pl-1">
              <li>to personalize your experience in order to better answer your needs</li>
              <li>to improve our website from the feedback you give us</li>
              <li>to improve customer service</li>
              <li>to process transactions, but your information will not be sold, traded, rented, given to any other third party other than for the purpose of delivering your purchase</li>
              <li>to send emails: the email address you provide for order processing, may be used to send you information and updates on your order</li>
              <li>to carry out a survey, a contest, a promotion.</li>
            </ul>
          </div>
        </b-col>
      </b-row>
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
  },
  methods: {
  }
}
</script>
