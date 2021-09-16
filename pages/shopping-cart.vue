<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
    <section class="pad-side wrapper-shopping">
      <b-container>
        <div class="d-flex align-items-center justify-content-between">
          <div class="title">SHOPPING CART</div>
        </div>
        <table class="table table-responsive shopping-cart mt-3">
          <thead>
            <tr>
              <th scope="col">PRODUCT</th>
              <th scope="col">NAME</th>
              <th scope="col">PRICE</th>
              <th scope="col">QUANTITY</th>
              <th scope="col">TOTAL</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>
                <img
                class="d-block img-fluid"
                src="/image-41.jpg"
                alt="image"
                />
              </td>
              <td>
                <div class="subtitle fw-600 mb-1">Travel Hammock</div>
                <div class="option">
                  <div>Size: Compact - 320x155cm / 10’5”x4’11”</div>
                  <div>Main Color: Turquoise</div>
                  <div>Accessories Hook: Hook</div>
                  <div>Accessories Sleeve: No Sleeve</div>
                </div>
              </td>
              <td>
                <div class="price">19.99 €</div>
              </td>
              <td>
                <div class="quantity counter">
                  <span @click="decrease">&minus;</span>
                  <span>{{counter}}</span>
                  <span @click="increase">&plus;</span>
                </div>
              </td>
              <td>
                <div class="total">19.99 €</div>
              </td>
            </tr>
            <tr>
              <td colspan="2"></td>
              <td colspan="2">
                <div class="subtitle fw-600 text-left pr-2">SUBTOTAL</div>
              </td>
              <td>19.99 €</td>
            </tr>
          </tbody>
        </table>
        <div class="text-right proced-checkout">
          <b-button variant="primary" class="mt-2" @click="$router.push('/shopping-cart-detail')">
            PROCED TO CHECKOUT
          </b-button>
        </div>
        
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
      counter: 1
    }
  },
  methods : {
    increase () {
      this.counter++
    },
    decrease () {
      this.counter--
    }
  }
}
</script>
