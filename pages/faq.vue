<template>
  <div>
    <!-- top bar -->
    <TopNavbar />

    <!-- navbar -->
    <Navbar />

    <!-- info -->
    <div class="static-info">
      <div class="position-relative">
        <img
        class="d-block w-100 img-auto"
        height="500"
        src="/image-40.jpg"
        alt="image"
        />
      </div>
    </div>

    <section class="pad-side">
      <div class="d-flex align-items-center justify-content-between">
        <div class="title">FAQ - FIND AN ANSWER</div>
        <div class="input-group search">
          <input type="text" class="form-control pl-1" placeholder="Search in questions…" aria-label="" aria-describedby="basic-addon1">
        </div>
      </div>
      <b-row class="mt-2">
        <b-col cols="5" class="mt-2">
          <div class="faq-category">
            <div class="title fs-1h fw-300">Product <br><span class="fw-400">Question</span></div>
          </div>
        </b-col>
        <b-col cols="7">
          <!-- desc accordion -->
          <div class="accordion faq">
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-1 variant="info" class="d-flex justify-between">
                  Why a Ticket to the Moon Hammock?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-1" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-2 variant="info" class="d-flex justify-between">
                  Do I need a Suspension System for my TTTM Hammock?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-3 variant="info" class="d-flex justify-between">
                  What is the Weight Limit for TTTM Products?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-4 variant="info" class="d-flex justify-between">
                  How many People fit in a TTTM Hammock?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-5 variant="info" class="d-flex justify-between">
                  Do you offer Warranty on your products?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-5" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-6 variant="info" class="d-flex justify-between">
                  Can I Make Love in a TTTM Hammock?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-6" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-7 variant="info" class="d-flex justify-between">
                  Are TTTM Hammocks Breathable?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-7" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-8 variant="info" class="d-flex justify-between">
                  How Do You Get in and Out a TTTM Hammock?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-8" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-9 variant="info" class="d-flex justify-between">
                  Why is there no Spreader Bar?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-9" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-10 variant="info" class="d-flex justify-between">
                  What is the Point of Using the Hook?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-10" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-11 variant="info" class="d-flex justify-between">
                  How much Space do I need to Hang my Hammock?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-11" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-12 variant="info" class="d-flex justify-between">
                  Can I use a standard Hammock Frame for my TTTM?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-12" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-13 variant="info" class="d-flex justify-between">
                  Does The Ticket To The Moon Mosquito Net 360° work with all TTTM Hammocks?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-13" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-14 variant="info" class="d-flex justify-between">
                  How do I wash my TTTM Hammock?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-14" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
          </div>
        </b-col>
      </b-row>
      <b-row class="mt-2">
        <b-col cols="5" class="mt-2">
          <div class="faq-category">
            <div class="title fs-1h fw-300">Product <br><span class="fw-400">Question</span></div>
          </div>
        </b-col>
        <b-col cols="7">
          <!-- desc accordion -->
          <div class="accordion faq">
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-1 variant="info" class="d-flex justify-between">
                  Is my order subject to import duties and other fees?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-1" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-2 variant="info" class="d-flex justify-between">
                  Is it safe to buy TTTM products online using a credit card?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-3 variant="info" class="d-flex justify-between">
                  Do you ship Everywhere?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-4 variant="info" class="d-flex justify-between">
                  How much do shipping and customs charges for my order cost?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-5 variant="info" class="d-flex justify-between">
                  How do I Track my order?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-5" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-6 variant="info" class="d-flex justify-between">
                  What payment options?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-6" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-7 variant="info" class="d-flex justify-between">
                  Can I pay using PayPal?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-7" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-8 variant="info" class="d-flex justify-between">
                  When will my order be shipped?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-8" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
          </div>
        </b-col>
      </b-row>
      <b-row class="mt-2">
        <b-col cols="5" class="mt-2">
          <div class="faq-category">
            <div class="title fs-1h fw-300">Product <br><span class="fw-400">Question</span></div>
          </div>
        </b-col>
        <b-col cols="7">
          <!-- desc accordion -->
          <div class="accordion faq" >
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-23 variant="info" class="d-flex justify-between">
                  How do I create an account?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-23" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-24 variant="info" class="d-flex justify-between">
                  Has my order been shipped yet?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-24" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-25 variant="info" class="d-flex justify-between">
                  How do I change quantities or items of my order?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-25" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-26 variant="info" class="d-flex justify-between">
                  How do I track my order?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-26" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
            <div no-body class="mb-1">
              <b-card-header header-tag="header" class="p-1" role="tab">
                <b-button block v-b-toggle.accordion-27 variant="info" class="d-flex justify-between">
                  How Do I Return or Exchange an Order?
                  <img
                    src="/plus.png"
                    alt="image"
                    height="12"
                  />
                </b-button>
              </b-card-header>
              <b-collapse id="accordion-27" accordion="my-accordion" role="tabpanel">
                <b-card-body>
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </b-card-body>
              </b-collapse>
            </div>
          </div>
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
      isHidden: false,
      categoryFAQ: [
        {
          name: 'PRODUCT QUESTIONS'
        },
        {
          name: 'INTERNATIONAL SHIPPING QUESTIONS'
        },
        {
          name: 'ORDER MANAGEMENT QUESTIONS'
        }
      ],
      selectedFAQ: 0
    }
  },
  methods: {
    onSelectFAQ (index) {
      this.selectedFAQ = index
    }
  }
}
</script>
