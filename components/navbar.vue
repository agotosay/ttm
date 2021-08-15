<template>
  <div class="top-bar sticky">
    <b-navbar toggleable="lg" type="light" variant="light">
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" class="justify-content-between" is-nav>
        <!-- Right aligned nav items -->
        <div class="input-group search">
          <div class="input-group-prepend">
            <img
            class="ml-1"
            src="/loupe.svg"
            height="14"
            alt="image"
            />
          </div>
          <input type="text" class="form-control" placeholder="" aria-label="Username" aria-describedby="basic-addon1">
        </div>
        <b-navbar-nav>
          <b-nav-item class="link-icon" href="#" v-on:click="isHidden = !isHidden">
            PRODUCTS
            <img
            class="ml-1"
            src="/arrow-down.svg"
            height="10"
            alt="image"
            />
          </b-nav-item>
          <b-nav-item href="#" @click="$router.push('/bundles')">BUNDLES</b-nav-item>
          <b-nav-item href="#" @click="$router.push('/about-us')">ABOUT US</b-nav-item>
          <b-nav-item href="#" @click="$router.push('/gallery')">GALLERY</b-nav-item>
          <b-nav-item href="#" class="ml-0" @click="$router.push('/contact-us')">CONTACT</b-nav-item>

        </b-navbar-nav>
        <b-nav pills class="navbar-right">
          <b-nav-item-dropdown
            id="my-nav-dropdown"
            text="EN"
            toggle-class="nav-link-custom"
            right
          >
            <b-dropdown-item>One</b-dropdown-item>
            <b-dropdown-item>Two</b-dropdown-item>
            <b-dropdown-divider></b-dropdown-divider>
            <b-dropdown-item>Three</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item-dropdown
            id="my-nav-dropdown"
            text="EUR"
            toggle-class="nav-link-custom"
            right
          >
            <b-dropdown-item>One</b-dropdown-item>
            <b-dropdown-item>Two</b-dropdown-item>
            <b-dropdown-divider></b-dropdown-divider>
            <b-dropdown-item>Three</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item @click="$router.push('/shopping-cart')">
            <img
            class="d-block img-margin"
            height="14"
            src="/cart.png"
            alt="image"
            />
          </b-nav-item>
          <b-nav-item class="user" @click="$router.push('/signIn')">
            <img
            class="d-block img-margin"
            height="14"
            src="/user.svg"
            alt="image"
            />
          </b-nav-item>
        </b-nav>
      </b-collapse>
    </b-navbar>

    <div class="mega-menu" v-if="isHidden">
      <b-container>
        <b-row>
          <b-col cols="3">
            <div class="title">Hammock</div>
            <ul>
              <li>
                <b-link>
                  Travel Hammock
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Lightest Hammock
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Pro Hammock
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="3">
            <div class="title">Hammock Chair</div>
            <ul>
              <li>
                <b-link>
                  Moon Chair
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Mini Moon Chair
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="3">
            <div class="title">Eco Backpack</div>
            <ul>
              <li>
                <b-link>
                  Mini Backpack 15 L
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Backpack Plus 25 L
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="3">
            <div class="title">Eco Shopping Bag</div>
            <ul>
              <li>
                <b-link>
                  Eco Bags
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
        </b-row>
        <b-row class="mt-2">
          <b-col cols="3">
            <div class="title">Hammock Accessories</div>
            <ul>
              <li>
                <b-link>
                  UV-Proof Hammock Sleeve
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Convertiblebug Net 360º
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Moonquilt
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Moontrap
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Fuul Moon Traap
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Lightest Trap
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="3">
            <div class="title">Hammock Suspension</div>
            <ul>
              <li>
                <b-link>
                  Moon Straps
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Lightest Strap
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Nautical Rope Kit
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="3">
            <div class="title">Tools</div>
            <ul>
              <li>
                <b-link>
                  Carabiner 10 KN
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Carabiner 22 KN
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  HAMMOCK ANCHOR KIT
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  RIDGELINE KIT
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="3">
            <div class="title">OTHERS</div>
            <ul>
              <li>
                <b-link>
                  POCKET FRISBEE
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  BEACH BLANKET
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  SLACKLINE
                  <img
                  class="ml-1"
                  src="/icon-hammock.svg"
                  height="12"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      isHidden: false
    }
  }
}
</script>