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
        <div class="title mb-2">ABOUT US</div>
        <p>TICKET TO THE MOON</p>
        <p>Ticket To The Moon is the original manufacturer of the camping hammock, based in Bali since 1996. As an ethical company, we love to think that we are more like some kind of tribe rather than just a business: not only do we develop and create innovative and useful products, but we also promote different ways of life.</p>
        <p>We are manufacturers of feel-good products for dreamers worldwide!</p>
        <p>PROVIDING SAFE, COMFORTABLE, HIGH QUALITY PRODUCTS</p>
        <p>Because we are the original inventors and manufacturers of the camping hammock, we give you the very best products and include the features you desire. The whole TTTM parachute product range is hand-made by a team of skilled craftsmen in our very own factory in Bali from the highest quality of nylon parachute fabric, locally sourced. Every one of our products is tested under extreme conditions, and passes strict quality control tests before it leaves our factory. The 10-year manufacturer’s warranty covers any defects in workmanship and materials on all Ticket To The Moon products. </p>
        <p>The signature range of TTTM hammocks is durable, elastic, breathable, anti-mildew, and skin-friendly (OEKO-TEX® Standard 100). The hammocks are available in five sizes and thousands of color combinations, and each comes with an attached pouch for easy traveling.</p>
        <p>Join The Hammock Tribe!</p>
        <p>LIGHTWEIGHT, COMPACT &amp; DURABLE</p>
        <p>The TTTM camping hammock is delivered in its own compact pouch, making it ideal as a travel bed, and perfect for taking a nap or just chilling. It makes for a marvelous playground too…</p>
        <p>The original TTTM set up system using stainless hooks and nautical ropes remains the easiest and safest available on the market. Another convenient way to set up your hammock uses high-grade carabiners & tree-friendly straps. Over the years, TTTM has developed a complete range of hammock, hammock accessories like The Tarp, The Mosquito Net 360° and The Carabiner, and a number of other lifestyle products such as the Moon Chair, the Beach Blanket, the Pocket Frisbee and our famous Eco-Friendly Bags. The high quality material and hand finish make all TTTM products suitable for an adventurer’s trip or for daily use.</p>
        <p>We like to make your life simpler!</p>
        <p>TICKET TO THE MOON &amp; CORPORATE SOCIAL RESPONSIBILITY</p>
        <p>It is important to us to offer original products that you will enjoy using, but we also aim to raise awareness of larger global challenges such as sustainability and fair trade production issues, while respecting local social structures and the Indonesian culture.</p>
        <p>At TTTM, there is absolutely no child labor. Our honest, humane, fair trade corporate values mean all staff enjoy proper working conditions with social security, a pension, and a basic salary that is far higher than the minimum salary. They only work five and a half 8-hour days per week, setting our company apart from most others and bonding workers into a unique social community. Since TTTM’s establishment in 1996, nobody has ever left the company despite attempts by copycats to lure them away.</p>
        <p>Please have a look inside the factory and headquarter of Bali, Indonesia.</p>
        <p>MINIMIZING OUR CORPORATE FOOTPRINT</p>
        <p>By using local materials and investing in innovative recycling methods, we aim to have a minimal impact on the environment. Any spare fabric left over after our unique products have been cut is turned into new merchandise like eco-friendly bags and backpacks. Our ongoing urge to minimize waste engendered the motto:  “No. No plastic bags, please!”</p>
        <p>We Care, Nothing is Left to Waste! </p>
        <p>TTTM FOUNDATION </p>
        <p>The Ticket To The Moon Foundation was established by notary deed in 2009. Our main purpose is to support the Sumbanese Kodi tribe in East Indonesia. We have developed health, educational, cultural and development aid programs, and to date we have successfully helped the local community with building new infrastructure and education facilities, malaria prevention programs, and access to clean water. </p>
        <p>We offer our business partners and other interested parties the same opportunity to help these remarkable people as part of corporate responsibility programs and donations. Ticket To The Moon is proud to have been part of this initiative since the beginning, and continues to contribute a significant portion of its net earnings to the Foundation.</p>
        <p>For more informatiom, click on ‘TTTM Foundation’.</p>
        <p>Keep your feet off the ground!!</p>
        <p>Charly – Founder of TICKETTOTHEMOON</p>
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
