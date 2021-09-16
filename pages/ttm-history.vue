<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
    <section class="ttm-history">
      <div class="title text-center mb-2">
        history of ticket to the moon
      </div>
      <b-row class="mb-4 mr-0">
        <b-col cols="12" md="6" lg="4" offset="4">
          <div class="info-contact text-center">
            <div class="title mb-2">{{selectedStep}}</div>
            <p>After a great initial success at many European music festivals, Charly realizes that his hammock could be something more than just a way to cover the costs of his travels…</p>
          </div>
        </b-col>
      </b-row>
      <div class="history-step">
        <div class="step" :class="{'active' : (2001 - (index-1)) === selectedStep }" v-for="index in 20" :key="index" @click="onSelectedStep(2001 - (index-1))">{{2001 - (index-1)}}</div>
      </div>
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
      selectedStep: 2001
    }
  },
  methods : {
    onSelectedStep (index) {
      this.selectedStep = index
    }
  }
}
</script>
