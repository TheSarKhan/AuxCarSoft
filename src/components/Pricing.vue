<script setup>
import { themeColor } from "../data/items";
const heading = "Pricing";
const subHeading = "Pricing for everyone. Choose your plan now!";
const startButtonName = "Get Started";
const packages = [
  {
    name: "Free",
    price: "0",
  },
  {
    name: "Standard",
    price: "19.99",
  },
  {
    name: "Premium",
    price: "79.99",
  },
];
</script>
<template>
  <div class="untree_co-section bg-light" id="pricing-section">
    <div class="container">
      <div class="row pricing-title">
        <div class="col-12 text-center" data-aos="fade-up" data-aos-delay="0">
          <h2 class="heading">{{ heading }}</h2>
          <p>{{ subHeading }}</p>
        </div>
      </div>
      <div class="row justify-content-center">
        <div class="col-lg-10">
          <div class="row">
            <div class="col-lg-4" data-aos="fade-up" data-aos-delay="100">
              <div class="pricing">
                <div class="body">
                  <div class="price">
                    <span class="d-block plan">{{ packages[0].name }}</span>
                    <span class="price" :style="[{ color: themeColor }]"
                      ><sup>$</sup><span>{{ packages[0].price }}</span></span
                    >
                  </div>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li>Access to basic tools</li>
                    <li>Limited dashboard features</li>
                    <li>Email support</li>
                    <li>Ideal for individuals testing our platform</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a
                      href="#"
                      class="btn btn-outline-primary"
                      :style="[
                        { color: themeColor },
                        { borderColor: themeColor },
                      ]"
                      >{{ startButtonName }}</a
                    >
                  </p>
                </div>
              </div>
            </div>
            <div class="col-lg-4" data-aos="fade-up" data-aos-delay="200">
              <div class="pricing active">
                <div class="body">
                  <div class="price">
                    <span class="d-block plan">{{ packages[1].name }}</span>
                    <span class="price" :style="[{ color: themeColor }]"
                      ><sup>$</sup><span>{{ packages[1].price }}</span></span
                    >
                  </div>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li>Full access to CRM and tracking tools</li>
                    <li>Custom website templates</li>
                    <li>Admin panel with limited modules</li>
                    <li>Email & chat support</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a
                      href="#"
                      class="btn btn-primary"
                      :style="[
                        { backgroundColor: themeColor },
                        { borderColor: themeColor },
                      ]"
                      >{{ startButtonName }}</a
                    >
                  </p>
                </div>
              </div>
            </div>
            <div class="col-lg-4" data-aos="fade-up" data-aos-delay="300">
              <div class="pricing">
                <div class="body">
                  <div class="price">
                    <span class="d-block plan">{{ packages[2].name }}</span>
                    <span class="price" :style="[{ color: themeColor }]"
                      ><sup>$</sup><span>{{ packages[2].price }}</span></span
                    >
                  </div>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li>All features unlocked</li>
                    <li>Advanced analytics & reporting</li>
                    <li>Custom-built dashboards</li>
                    <li>Priority support</li>
                    <li>Ideal for logistics teams and businesses</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a
                      href="#"
                      class="btn btn-outline-primary"
                      :style="[
                        { color: themeColor },
                        { borderColor: themeColor },
                      ]"
                      >{{ startButtonName }}</a
                    >
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
