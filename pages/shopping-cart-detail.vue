<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
    <section class="pad-side">
      <b-container>
        <b-row>
          <b-col cols="6" class="pr-2">
            <div class="title fs-2 mb-1">Billing &amp; Shipping Address</div>
            <p>Click Here To Login Or Fill Input Below</p>
            <div class="subtitle fw-500 mt-2 mb-1 text-uppercase">Shipping information :</div>
            <b-form class="mb-1">
              <label>First name :</label>
              <b-form-input type="text" id="first-name" placeholder="First name" class="rounded-radius"/>
            </b-form>
            <b-form class="mb-1">
              <label>Last name :</label>
              <b-form-input type="text" id="last-name" placeholder="Last name" class="rounded-radius"/>
            </b-form>
            <b-form class="mb-1">
              <label>Postal Code :</label>
              <b-form-input type="number" id="postal-code" placeholder="Postal code" class="rounded-radius"/>
            </b-form>
            <b-form class="mb-1">
              <label>Address Line 1 :</label>
              <b-form-input type="text" id="address-1" placeholder="Address" class="rounded-radius"/>
            </b-form>
            <b-form class="mb-1">
              <label>Address Line 2 (Optional) :</label>
              <b-form-input type="text" id="address-2" placeholder="Address" class="rounded-radius"/>
            </b-form>
            <b-row>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>State :</label>
                  <b-form-input type="number" id="state" placeholder="State" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>Country :</label>
                  <b-form-select v-model="selected" :options="options" class="mb-1 rounded-radius"></b-form-select>
                </b-form>
              </b-col>
            </b-row>
            <small>* If you don't find your country in the list, Please reach out to us through the <b-link class="fw-500" @click="$router.push('/contact-us')">CONTACT US</b-link> page</small>
            <div class="title fs-2 mt-2 mb-1">Billing Information</div>
            <b-form-checkbox
              id="checkbox-1"
              name="checkbox-1"
              value="accepted"
              unchecked-value="not_accepted"
            >
              Billing Address Same As Shipping Address
            </b-form-checkbox>
            <div class="title fs-2 mt-2">Checkout As</div>
            <div class="d-flex w-100 mt-0h">
              <b-form-radio name="some-radios" value="A" class="mr-1">Guest</b-form-radio>
              <b-form-radio name="some-radios" value="B">Create an Account</b-form-radio>
            </div>
            <div class="title fs-2 mt-2 mb-1">Additional Info</div>
            <b-form-textarea
              id="textarea"
              placeholder="Comment"
              rows="6"
              max-rows="9"
            ></b-form-textarea>
            <div class="title fs-2 mt-2 mb-1">Promotion Code / Voucher</div>
            <div class="d-flex align-items-center">
              <input id="search-1" type="text" placeholder="enter code" class="form-subscribe form-control rounded-radius">
              <b-button variant="primary" class="ml-1">APPLY</b-button>
            </div>
          </b-col>
          <b-col cols="6" class="pl-2">
            <div class="title fs-2 mb-1">Choose Payment Method</div>
            <div class="w-100 mt-0h">
              <b-form-radio name="some-radios" value="A" class="mr-1 d-flex mb-1">
                CREDIT OR DEBIT CARDS 
                <img
                class="ml-2"
                src="/logo-cc.jpg"
                height="30"
                alt="image"
                />
              </b-form-radio>
              <b-form-radio name="some-radios" value="B">
                PAYPAL <small>( We Accept Paypal. )</small>
              </b-form-radio>
            </div>
            <div class="subtitle fw-500 mt-3 mb-1 text-uppercase mt-2">ORDER SUMMARY</div>
            <div class="order-summary d-flex align-items-center justify-content-between">
              <img
                class="d-block img-fluid"
                src="/image-41.jpg"
                alt="image"
              />
              <div class="info ml-2">
                <div class="subtitle fw-500 mb-0h">Travel Hammock</div>
                <p>Size Eco Backpack: Eco Backpack Size Main Color Eco Backpack: Blue Second Color Eco Backpack: Aqua</p>
                <b-link class="mt-1">Edit Chart</b-link>
              </div>
            </div>
            <div class="subtitle fw-500 mt-3 mb-1 text-uppercase mt-2">SUMMARY</div>
            <div class="summary mb-2">
              <div class="list d-flex justify-content-between mb-1 align-items-start">
                <div class="subtitle">SUBTOTAL</div>
                <div class="price">19.99 €</div>
              </div>
              <div class="list d-flex justify-content-between mb-1 align-items-start">
                <div class="subtitle">VAT (10%)</div>
                <div class="price">FREE</div>
              </div>
              <div class="list d-flex justify-content-between mb-1 align-items-start">
                <div class="subtitle">
                  SHIPPING AND IMPORT FEES TO YOUR COUNTRY <br />
                  <small>World Wide Shipping</small> 
                </div>
                <div class="price">FREE</div>
              </div>
              <div class="list d-flex justify-content-between mb-1 align-items-start">
                <b-form-radio name="some-radios2" value="A" class="mr-1">Express - TNT / FEDEX - 5-7 Business Days</b-form-radio>
                <div class="price">9 €</div>
              </div>
              <div class="list d-flex justify-content-between mb-1 align-items-start">
                <div class="subtitle">Total</div>
                <div class="price">19.99 €</div>
              </div>
            </div>
            <b-form-checkbox
              id="checkbox-2"
              name="checkbox-2"
              value="accepted"
              class="mb-1"
              unchecked-value="not_accepted"
            >
              Subscribe to our newsletter
            </b-form-checkbox>
            <b-form-checkbox
              id="checkbox-3"
              name="checkbox-3"
              value="accepted"
              unchecked-value="not_accepted"
            >
              Please use a correct address detail and telephone number so that the delivery service can reach you, otherwise your products will not arrive at destination
            </b-form-checkbox>
            <b-button variant="primary" class="mt-2">Continue</b-button>
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
      selected: null,
      options: [
        { value: null, text: 'Please select' },
        { value: 'a', text: 'Option A' },
        { value: 'b', text: 'Option B' },
        { value: 'c', text: 'Option C' },
      ]
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
