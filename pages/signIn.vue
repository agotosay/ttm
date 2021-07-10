<template>
  <div>
    <b-row>
      <b-col cols="7" class="pr-0 pl-0">
        <img
        class="d-block w-100 img-signIn"
        src="/img-signin.png"
        alt="image"
        />
      </b-col>
      <b-col cols="5" class="pr-0 pl-0 signIn">
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
              <b-form-radio name="some-radios" value="A">Option A</b-form-radio>
              <b-form-radio name="some-radios" value="B">Option B</b-form-radio>
            </div>
          </b-form-group>
          <b-form-group>
            <b-form-input
              id="input-1"
              type="email"
              placeholder="Enter email"
            ></b-form-input>
            <b-form-input
              placeholder="Password"
              type="password"
              id="text-password"
              class="mt-1"></b-form-input>
          </b-form-group>
          <div class="button-login">
            <b-button variant="primary" class="d-block">Login</b-button>
            <b-button variant="secondary" class="d-block mt-1">register</b-button>
          </div>
          <div class="forgot">
            <b-link>Forgot Password?</b-link>
            <b-link>Signup</b-link>
          </div>
        </div>
      </b-col>
    </b-row>
  </div>
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
