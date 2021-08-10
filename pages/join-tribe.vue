<template>
  <div>
  <!-- top bar -->
  <TopNavbar />

  <!-- navbar -->
  <Navbar />

  <!-- info -->
  <section>
    <b-container class="gallery">
      <div class="title mb-2">
        Join the tribe
      </div>
      <b-row class="mt-2">
        <b-col cols="6">
          <b-form class="mb-1">
            <label>Full name :</label>
            <b-form-input type="text" id="full-name" placeholder="Full name" class="rounded-radius"/>
          </b-form>
          <b-form class="mb-1">
            <label>Phone :</label>
            <b-form-input type="text" id="for-phone" placeholder="Phone" class="rounded-radius"/>
          </b-form>
          <b-form class="mb-1">
            <label>Type &amp; color of hammock :</label>
            <b-form-input type="text" id="last-name" placeholder="Type &amp; Color Of Hammock" class="rounded-radius"/>
          </b-form>
          <b-form-group>
            <label>How do you know about us? :</label>
            <div class="w-100 mt-0h">
              <b-form-radio name="some-radios" value="A" class="mr-1">Friends /Family</b-form-radio>
              <b-form-radio name="some-radios" value="B" class="mr-1">Shop / Reseller</b-form-radio>
              <b-form-radio name="some-radios" value="C" class="mr-1">Facebook</b-form-radio>
              <b-form-radio name="some-radios" value="D" class="mr-1">Instagram</b-form-radio>
              <b-form-radio name="some-radios" value="E" class="mr-1">Pinterest</b-form-radio>
              <b-form-radio name="some-radios" value="F" class="mr-1">Other</b-form-radio>
            </div>
          </b-form-group>
        </b-col>
        <b-col cols="6">
          <b-form class="mb-1">
            <label>Email :</label>
            <b-form-input type="email" id="for-email" placeholder="Email" class="rounded-radius"/>
          </b-form>
          <b-form class="mb-1">
            <label>Date purchase :</label>
            <b-form-input type="date" id="for-email" placeholder="dd/mm/yyyy" class="rounded-radius"/>
          </b-form>
          <b-form class="mb-1">
            <label>Place of purchase :</label>
            <b-form-input type="email" id="for-email" placeholder="Place Of Purchase" class="rounded-radius"/>
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
