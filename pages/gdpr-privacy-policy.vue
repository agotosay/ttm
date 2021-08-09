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
        <div class="title mb-2">GDPR PRIVAY POLICY</div>
        <div class="subtitle mb-1">DEFINITIONS</div>
        <ul class="pl-1 definitions">
          <li>
            TICKET TO THE MOON Trademark<br />
            PT. Ayunan Bulan International<br />
            Jalan Batu Sangian VI No.10, 80361 Bali, Indonesia
          </li>
          <li>
            GDPR<br />
            General Data Protection Regulation Act.
          </li>
          <li>
            Data Controller<br />
            Data controller means the natural or legal person who(oether alone or jointhly or in common with other persons) determines the purposes for which and the manner in which any personal information are, or are to be, processed.
          </li>
          <li>
            Data Processor<br />
            Data Processor means any natural or legal person who processes the data on behalf of the Data Controller.
          </li>
          <li>
            Data Subject<br/>
            Data Subject is any living individual who is using our Service and is the subject of Personal Data.
          </li>
        </ul>
        <div class="mt-3">
          <b-row>
            <b-col cols="6">
              <ul class="pl-1 left-tab">
                <li>Principles for processing personal data</li>
                <li>What personal data we collcet and process</li>
                <li>How we use the personal data</li>
                <li>Legal basis for collecting and processing personal data</li>
                <li>Retention of personal data</li>
              </ul>
            </b-col>
            <b-col cols="6">
              <div class="fw-500 mb-1">Our priciples for processing personal data are:</div>
              <ul class="pl-1">
                <li>Fairness and lawfulness.</li>
                <li>When we process personal data, the individual rights of the Data Subjects must be protected.</li>
                <li>All personal data must be collected and processed in a legal and fair manner.<br /> Restricted to a specific purpose.</li>
                <li>The Personal data of Data Subject must be processed only for specific purposes.<br /> Transparency.</li>
                <li>The Data Subject must be informed of how his/her data is being collected, processed and used.</li>
              </ul>
            </b-col>
          </b-row>
        </div>
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
    }
}
