<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
    <section class="cart-detail">
      <b-row>
        <b-col cols="7" class="pr-2 cols">
          <div class="subtitle fs-1h mb-1">Shipping Details</div>
          <hr />
          <p class="mt-2">Click Here To Login Or Fill Input Below</p>
          <div class="subtitle fw-500 mb-1 text-uppercase">Shipping information :</div>
          <b-row>
            <b-col cols="6">
              <b-form class="mb-1">
                <label>First name :</label>
                <b-form-input type="text" id="first-name" placeholder="" class="rounded-radius"/>
              </b-form>
              <b-form class="mb-1">
                <label>Email :</label>
                <b-form-input type="email" id="email" placeholder="" class="rounded-radius"/>
              </b-form>
            </b-col>
            <b-col cols="6">
              <b-form class="mb-1">
                <label>Last name :</label>
                <b-form-input type="text" id="last-name" placeholder="" class="rounded-radius"/>
              </b-form>
              <b-form class="mb-1">
                <label>Phone :</label>
                <b-form-input type="tel" id="phone" placeholder="" class="rounded-radius"/>
              </b-form>
            </b-col>
            <b-col cols="12">
              <b-form class="mb-1">
                <label>Address:</label>
                <b-form-input type="text" id="address-1" class="rounded-radius"/>
              </b-form>
            </b-col>
            <b-col cols="6">
              <b-form class="mb-1">
                <label>Zip Code :</label>
                <b-form-input type="number" id="postal-code" placeholder="" class="rounded-radius"/>
              </b-form>
              <b-form class="mb-1">
                <label>State :</label>
                <b-form-input type="number" id="state" placeholder="" class="rounded-radius"/>
              </b-form>
            </b-col>
            <b-col cols="6">
              <b-form class="mb-1">
                <label>City :</label>
                <b-form-input type="number" id="postal-code" placeholder="" class="rounded-radius"/>
              </b-form>
              <b-form class="mb-1">
                <label>Country :</label>
                <b-form-select v-model="selected" :options="options" class="mb-1 rounded-radius"></b-form-select>
              </b-form>
            </b-col>
          </b-row>
          <small>* If you don't find your country in the list, Please reach out to us through the <b-link class="fw-500" @click="$router.push('/contact-us')">CONTACT US</b-link> page</small>
          <div class="subtitle fs-1h mt-2 mb-1">Billing Information</div>
          <b-form-checkbox
            id="checkbox-1"
            name="checkbox-1"
            value="accepted"
            unchecked-value="not_accepted"
            v-model="billingAddress"
          >
            Billing Address Same As Shipping Address
          </b-form-checkbox>
          <div v-if="billingAddress !== 'accepted'" class="mt-1">
            <b-row>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>First name :</label>
                  <b-form-input type="text" id="first-name" placeholder="" class="rounded-radius"/>
                </b-form>
                <b-form class="mb-1">
                  <label>Email :</label>
                  <b-form-input type="email" id="email" placeholder="" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>Last name :</label>
                  <b-form-input type="text" id="last-name" placeholder="" class="rounded-radius"/>
                </b-form>
                <b-form class="mb-1">
                  <label>Phone :</label>
                  <b-form-input type="tel" id="phone" placeholder="" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="12">
                <b-form class="mb-1">
                  <label>Address:</label>
                  <b-form-input type="text" id="address-1" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>Zip Code :</label>
                  <b-form-input type="number" id="postal-code" placeholder="" class="rounded-radius"/>
                </b-form>
                <b-form class="mb-1">
                  <label>State :</label>
                  <b-form-input type="number" id="state" placeholder="" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>City :</label>
                  <b-form-input type="number" id="postal-code" placeholder="" class="rounded-radius"/>
                </b-form>
                <b-form class="mb-1">
                  <label>Country :</label>
                  <b-form-select v-model="selected" :options="options" class="mb-1 rounded-radius"></b-form-select>
                </b-form>
              </b-col>
            </b-row>
          </div>
          <div class="subtitle fs-1h mt-2">Checkout As</div>
          <div class="d-flex w-100 mt-0h">
            <b-form-radio name="for-checkout" value="guest" class="mr-1" v-model="checkoutAs">Guest</b-form-radio>
            <b-form-radio name="for-checkout" value="newaccount" v-model="checkoutAs">Create an Account</b-form-radio>
          </div>
          <div v-if="checkoutAs === 'newaccount'" class="mt-1">
            <b-row>
              <b-col cols="12">
                <b-form class="mb-1">
                  <label>Email :</label>
                  <b-form-input type="email" id="email" placeholder="" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>Password :</label>
                  <b-form-input type="passowrd" id="password" placeholder="" class="rounded-radius"/>
                </b-form>
              </b-col>
              <b-col cols="6">
                <b-form class="mb-1">
                  <label>Retype Password :</label>
                  <b-form-input type="passowrd" id="retype-password" placeholder="" class="rounded-radius"/>
                </b-form>
              </b-col>
            </b-row>
          </div>
          <div class="subtitle fs-1h mt-2">Choose Payment Method</div>
          <div class="w-100 mt-0h">
            <b-form-radio v-model="forPayment" name="for-payment" v-bind:value="'cc'" class="mr-1 d-flex mb-1">
              CREDIT OR DEBIT CARDS 
              <img
              class="ml-2"
              src="/logo-cc.jpg"
              height="30"
              alt="image"
              />
            </b-form-radio>
            <div v-if="forPayment === 'cc'" class="mt-1 mb-3">
              <small>We Accept All Major Credit And Debit Cards With Secure Online Payment System Processed Through Stripe</small>
              <b-row class="d-flex align-items-center">
                <b-col cols="9">
                  <b-form class="mb-1 mt-1">
                    <label>Card Number :</label>
                    <b-form-input type="number" id="card-number" class="rounded-radius"/>
                  </b-form>
                </b-col>
                <b-col cols="3" class="mt-2">
                  <img
                  class="ml-2"
                  src="/visa.png"
                  height="40"
                  alt="image"
                  />
                </b-col>
                <b-col cols="12">
                  <b-form class="mb-1">
                    <label>Name on Card:</label>
                    <b-form-input type="text" id="card-name" class="rounded-radius"/>
                  </b-form>
                </b-col>
                <b-col cols="3">
                  <b-form class="mb-1">
                    <label>Expiration Date:</label>
                    <b-form-input type="number" id="card-month" placeholder="MM" class="rounded-radius"/>
                  </b-form>
                </b-col>
                <b-col cols="3">
                  <b-form class="mb-1">
                    <label class="label-transpatent">-</label>
                    <b-form-input type="number" id="card-year" placeholder="YY" class="rounded-radius"/>
                  </b-form>
                </b-col>
                <b-col cols="3">
                  <b-form class="mb-1">
                    <label>CVC:</label>
                    <b-form-input type="number" id="card-cvc" placeholder="XXX" class="rounded-radius"/>
                  </b-form>
                </b-col>
              </b-row>
            </div>
            <b-form-radio v-model="forPayment" name="for-payment" v-bind:value="'paypal'">
              PAYPAL <small>( We Accept Paypal. )</small>
              <img
              class="ml-2"
              src="/paypal.png"
              height="20"
              alt="image"
              />
            </b-form-radio>
          </div>
        </b-col>
        <b-col cols="5" class="pl-2 cols bc-grey">
          <div class="subtitle fs-1h mb-1">Promotion Code / Voucher</div>
          <hr />
          <div class="d-flex align-items-center">
            <input id="search-1" type="text" placeholder="enter code" class="form-subscribe form-control rounded-radius bc-transparent">
            <b-button variant="primary" class="ml-1">APPLY</b-button>
          </div>
          <div class="subtitle fs-1h mb-1 mt-2">Order Note</div>
          <hr />
          <b-form-textarea
            id="textarea"
            class="rounded-radius bc-transparent"
            placeholder="Additional note for your order"
            rows="6"
            max-rows="9"
          ></b-form-textarea>
          
          <div class="subtitle fs-1h mb-1 mt-2">ORDER SUMMARY</div>
          <hr />
          <b-row>
            <b-col cols="6">
              Product
            </b-col>
            <b-col cols="3">
              QTY
            </b-col>
            <b-col cols="3" class="text-right">
              Total
            </b-col>
          </b-row>
          <b-row class="mt-1">
            <b-col cols="6">
              <div class="fw-500">Travel Hammock</div>
              <div><span class="fw-500">Size: </span>Compact - 320x155cm / 10’5”x4’11”</div>
              <div><span class="fw-500">Main Color: </span>Turquoise</div>
              <div><span class="fw-500">Accessories Hook: </span>Hook</div>
              <div><span class="fw-500">Accessories Sleeve: </span> No Sleeve</div>
            </b-col>
            <b-col cols="3">
              1
            </b-col>
            <b-col cols="3" class="text-right">
              59,95 &euro;
            </b-col>
          </b-row>
          <hr>
          <div class="summary mb-2">
            <div class="list d-flex justify-content-between mb-1 align-items-start">
              <div class="subtitle fw-500">SUBTOTAL</div>
              <div class="price">59,95 &euro;</div>
            </div>
            <hr>
            <div class="list d-flex justify-content-between mb-1 align-items-start">
              <div class="subtitle fw-500">VAT (10%)</div>
              <div class="price">9 &euro;</div>
            </div>
            <hr>
            <div class="list d-flex justify-content-between mb-1 align-items-start">
              <div class="subtitle">
                <span class="fw-500">SHIPPING AND IMPORT FEES TO YOUR COUNTRY </span><br />
                <small>World Wide Shipping</small> 
              </div>
              <div class="price">9 &euro;</div>
            </div>
            <div class="list d-flex justify-content-between mb-1 align-items-start">
              <b-form-radio name="some-radios2" value="accepted" class="mr-1" v-model="shippingBy">Express - TNT / FEDEX - 5-7 Business Days</b-form-radio>
            </div>
            <hr>
            <div class="list d-flex justify-content-between mb-1 align-items-start">
              <div class="subtitle fw-500">Total</div>
              <div class="price">77.95 &euro;</div>
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
          <b-button variant="primary" class="mt-2 w-100">Continue</b-button>
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
      selected: null,
      forPayment: '',
      billingAddress: 'accepted',
      checkoutAs: 'guest',
      shippingBy: 'accepted',
      options: [
        { value: null, text: '' },
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
