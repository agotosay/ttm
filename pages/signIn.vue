<template>
  <b-container>
    <b-row class="box-signIn">
      <b-col cols="12" lg="7" class="pr-0 pl-0 img-signIn">
        <img
        class="d-block w-100 img-signIn"
        src="/img-signin.png"
        alt="image"
        />
      </b-col>
      <b-col cols="12" md="12" lg="5" class="pr-0 pl-0 signIn">
        <div class="box">
          <img
            class="d-block img-margin"
            src="/black-logo.png"
            height="22"
            alt="image"
          />
          <label class="d-block text-center mt-2">Login as</label>
          <b-form-group class="d-flex justify-content-center">
            <div class="d-flex w-100 mb-2">
              <b-form-radio name="some-radios" value="A">Customer</b-form-radio>
              <b-form-radio name="some-radios" value="B">Ambassador</b-form-radio>
            </div>
          </b-form-group>
          <b-form-group>
            <b-form-input
              class="rounded-radius"
              id="input-1"
              type="email"
              placeholder="Enter email"
            ></b-form-input>
            <b-form-input
              placeholder="Password"
              type="password"
              id="text-password"
              class="mt-1 rounded-radius"></b-form-input>
          </b-form-group>
          <b-row>
            <b-col cols="12" md="12" lg="8" offset="2">
              <div class="button-login">
                <b-button variant="primary" class="d-block">Login</b-button>
                <b-button variant="primary2" class="d-block mt-1">register</b-button>
              </div>
              <div class="forgot">
                <b-link>Forgot Password?</b-link>
                <b-link>Signup</b-link>
              </div>
            </b-col>
          </b-row>
        </div>
      </b-col>
    </b-row>
  </b-container>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Alegreya+Sans:wght@300;400;500;600;900&display=swap");
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css");
</style>

<script>
export default {
  data() {
    return {
      selected: ''
    }
  }
}
</script>
