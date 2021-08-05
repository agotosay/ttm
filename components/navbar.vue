<template>
  <div class="position-relative">
    <b-navbar toggleable="lg" type="light" variant="light">
      <b-navbar-brand @click="$router.push('/')" class="logo">
        <img
        class="d-block img-margin"
        src="/black-logo.png"
        height="20"
        alt="image"
        />
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#" v-on:click="isHidden = !isHidden">PRODUCTS</b-nav-item>
          <b-nav-item href="#">SHOP</b-nav-item>
          <b-nav-item href="#">BUNDLES</b-nav-item>
          <b-nav-item href="#">ABOUT US</b-nav-item>
          <b-nav-item href="#">GALLERY</b-nav-item>
          <b-nav-item href="#">CONTACT</b-nav-item>
          <b-nav-item to="/signIn">
            <b-img src="../static/shopping-bag.svg" fluid alt="" width="14"></b-img>
          </b-nav-item>

        </b-navbar-nav>
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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
                  src="/arrow-right.svg"
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