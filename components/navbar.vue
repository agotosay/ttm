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
        <b-navbar-nav class="middle">
          <b-nav-item class="link-icon" href="#" @click="isHidden = !isHidden">
            PRODUCTS
            <img
            class="ml-0h mr-0h"
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
        <div class="navbar-right">
          <ul class="navbar-nav">
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle d-flex align-items-center" role="button" data-bs-toggle="dropdown" aria-expanded="false" @click="dropDown">
                <img
                src="/en.png"
                height="16"
                alt="image"
                />
                <span class="ml-0h">EN</span>
              </a>
              <ul class="dropdown-menu" :class="{'show': showDropdown}">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><hr class="dropdown-divider"></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle d-flex align-items-center" id="asd2" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                <span>EUR</span>
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Action</a></li>
                <li><a class="dropdown-item" href="#">Another action</a></li>
                <li><hr class="dropdown-divider"></li>
                <li><a class="dropdown-item" href="#">Something else here</a></li>
              </ul>
            </li>
            <li class="nav-item cart pointer" @click="$router.push('/shopping-cart')">
              <div class="counter">2</div>
              <img
              class="d-block img-margin ml-1 mr-1"
              height="14"
              src="/cart.png"
              alt="image"
              />
            </li>
            <li class="nav-item user pointer" @click="$router.push('/signIn')">
              <img
              class="d-block img-margin"
              height="14"
              src="/user.svg"
              alt="image"
              />
            </li>
          </ul>
        </div>
      </b-collapse>
    </b-navbar>

    <div class="mega-menu" v-if="isHidden">
      <b-container>
        <b-row>
          <b-col cols="12" lg="3">
            <div class="title">Hammock</div>
            <ul>
              <li>
                <b-link>
                  Travel Hammock
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-travel-hammock.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Lightest Hammock
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-lightest-hammock.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Pro Hammock
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-pro-hammock.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="12" lg="3">
            <div class="title">Hammock Chair</div>
            <ul>
              <li>
                <b-link>
                  Moon Chair
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-moon-chair.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Mini Moon Chair
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-mini-moon-chair.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="12" lg="3">
            <div class="title">Eco Backpack</div>
            <ul>
              <li>
                <b-link>
                  Mini Backpack 15 L
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-mini-backpack-15L.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Backpack Plus 25 L
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-backpack-plus-25L.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="12" lg="3">
            <div class="title">Eco Shopping Bag</div>
            <ul>
              <li>
                <b-link>
                  Eco Bags
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-eco-bags.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
        </b-row>
        <b-row class="mt-2">
          <b-col cols="12" lg="3">
            <div class="title">Hammock Accessories</div>
            <ul>
              <li>
                <b-link>
                  UV-Proof Hammock Sleeve
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-uv-proof-hammock-sleeve.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Convertiblebug Net 360º
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-convertible-bug-net.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Moonquilt
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-moonquilt.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Moontrap
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-moontarp.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Fuul Moon Trap
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-fullmoon-tarp.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Lightest Trap
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-lightest-tarp.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="12" lg="3">
            <div class="title">Hammock Suspension</div>
            <ul>
              <li>
                <b-link>
                  Moon Straps
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-moon-strap.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Lightest Strap
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-lightest-strap.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Nautical Rope Kit
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-naughtical-rope-kit.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="12" lg="3">
            <div class="title">Tools</div>
            <ul>
              <li>
                <b-link>
                  Carabiner 10 KN
                  <img
                  class="ml-1"
                  src="/menu-icon/carabiner-10kn.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  Carabiner 22 KN
                  <img
                  class="ml-1"
                  src="/menu-icon/carabiner-22kn.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  HAMMOCK ANCHOR KIT
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-hammock-anchor-kit.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  RIDGELINE KIT
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-ridgeline-kit.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
          <b-col cols="12" lg="3">
            <div class="title">OTHERS</div>
            <ul>
              <li>
                <b-link>
                  POCKET FRISBEE
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-pocket-frisbee.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  BEACH BLANKET
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-beach-blanket.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
              <li>
                <b-link>
                  SLACKLINE
                  <img
                  class="ml-1"
                  src="/menu-icon/icon-slackline.png"
                  height="28"
                  alt="image"
                  />
                </b-link>
              </li>
            </ul>
          </b-col>
        </b-row>
        <div class="close-menu" @click="closeMegamenu">
          <img
            class="d-block img-fluid"
            src="/cancel.svg"
            alt="image"
          />
        </div>
      </b-container>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      isHidden: false,
      showDropdown: false
    }
  },
  methods: {
    dropDown() {
      this.showDropdown = !this.showDropdown
    },
    closeMegamenu() {
      this.isHidden = false
    }
  }
}
</script>