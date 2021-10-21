<template>
  <div class="home">
    <section class="hero is-white is-fullheight">
      <div class="hero-body">
        <div class="container">
          <div class="columns is-vcentered reverse-columns">
            <div
              class="
                column
                is-10-mobile
                is-offset-1-mobile
                is-10-tablet
                is-offset-1-tablet
                is-5-desktop
                is-offset-1-desktop
                is-5-widescreen
                is-offset-1-widescreen
                is-5-fullhd
                is-offset-1-fullhd
              "
              data-aos="fade-down"
            >
              <h4 class="title titled is-1 mb-6">
                PivoHub
              </h4>
              <h2
                class="
                  subtitled
                  subtitle
                  has-text-grey
                  is-4
                  has-text-weight-normal
                  is-family-sans-serif
                "
              >
                People deserve to discover the story of a human industry that
                cares about its craft. PivoHub provides powerful and simple
                software to create a digital ecosystem that connects, organizes,
                and equips the craft beverage industry. We will be the
                best-of-breed craft beverage marketplace working with the
                world’s most notorious artisans.
              </h2>
              <div class="buttons">
                <b-button
                  class="button is-primary is-rounded"
                  to="/sell"
                  @click="showRegister = true"
                  size="is-large"
                  >Sell</b-button
                >

                <router-link to="/buy">
                  <b-button
                    class="button isrounded is-outlined is-rounded"
                    size="is-large"
                    >Buy</b-button
                  >
                </router-link>
              </div>
            </div>
            <div
              data-aos="fade-right"
              class="
                column
                is-10-mobile
                is-offset-1-mobile
                is-10-tablet
                is-offset-1-tablet
                is-4-desktop
                is-offset-1-desktop
                is-4-widescreen
                is-offset-1-widescreen
                is-4-fullhd
                is-offset-1-fullhd
              "
            >
              <figure>
                <img src="@/assets/img/undraw_refreshing.svg" />
              </figure>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="hero is-white is-fullheight">
      <div class="hero-body">
        <div class="container">
          <div class="columns is-vcentered">
            <div
              data-aos="fade-left"
              class="
                column
                is-10-mobile
                is-offset-1-mobile
                is-10-tablet
                is-offset-1-tablet
                is-4-desktop
                is-offset-1-desktop
                is-4-widescreen
                is-offset-1-widescreen
                is-4-fullhd
                is-offset-1-fullhd
              "
            >
              <figure class="image is-square">
                <img src="@/assets/img/undraw_wine.svg" />
              </figure>
            </div>
            <div
              data-aos="fade-down"
              class="
                column
                is-10-mobile
                is-offset-1-mobile
                is-10-tablet
                is-offset-1-tablet
                is-5-desktop
                is-offset-1-desktop
                is-5-widescreen
                is-offset-1-widescreen
                is-5-fullhd
                is-offset-1-fullhd
              "
            >
              <h1 class="title titled is-1 mb-6">
                Order management
              </h1>
              <h2
                class="
                  subtitled
                  subtitle
                  has-text-grey
                  is-4
                  has-text-weight-normal
                  is-family-sans-serif
                "
              >
                Get discovered by thousands of retailers with an online
                catalogue that's shows buyers exactly what they're getting.
                Adjust pricing, hide and display products by customer, and send
                special offers to the ones you love.Your inventory updates with
                every order, showing your clients and distributors exactly
                what's in stock in real time.
              </h2>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="hero is-white is-fullheight">
      <div class="hero-body">
        <div class="container">
          <div class="columns is-vcentered reverse-columns">
            <div
              data-aos="fade-right"
              class="
                column
                is-10-mobile
                is-offset-1-mobile
                is-10-tablet
                is-offset-1-tablet
                is-5-desktop
                is-offset-1-desktop
                is-5-widescreen
                is-offset-1-widescreen
                is-5-fullhd
                is-offset-1-fullhd
              "
            >
              <h1 class="title titled is-1 mb-6">
                Keep everything in sync
              </h1>
              <h2
                class="
                  subtitled
                  subtitle
                  has-text-grey
                  is-4
                  has-text-weight-normal
                  is-family-sans-serif
                "
              >
                Online Marketplace Showcase your products to thousands of
                retailers. Real-Time Inventory Update your inventory
                automatically with every order and every return. Performance
                Dashboard Keep track of your top products and best customers.
              </h2>
            </div>
            <div
              data-aos="fade-down fade-up"
              class="
                column
                is-10-mobile
                is-offset-1-mobile
                is-10-tablet
                is-offset-1-tablet
                is-4-desktop
                is-offset-1-desktop
                is-4-widescreen
                is-offset-1-widescreen
                is-4-fullhd
                is-offset-1-fullhd
              "
            >
              <figure class="image is-square">
                <img src="@/assets/img/undraw_beer.svg" />
              </figure>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="container">
      <div data-aos="fade-up" class="box cta">
        <p class="has-text-centered">
          <span class="tag is-primary">New</span> This Part Will include all the
          news about the company and upcoming changes
        </p>
      </div>
      <div data-aos="fade-right" class="intro column is-8 is-offset-2">
        <b-button class="button is-primary is-rounded" to="/buy" size="is-large"
          >Buy</b-button
        >
        <br />
        <br />
        <br />
        <p data-aos="fade-down" class="title">
          Order anytime, anywhere... <br />Even on the 🚽😂
        </p>
        <br />
      </div>
    </section>
    <section class="container">
      <div class="columns features">
        <div class="column is-4">
          <div data-aos="fade-right" class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fas fa-smile"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>
                  Discover what's new, Re-order your products with an amazing
                  Dashboard
                </h4>
                <p>
                  Trash the paper catalogues and know what your customers really
                  like, Keep track update and understand the customer using our
                  new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
        <div class="column is-4">
          <div data-aos="fade-up" class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fas fa-smile"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>
                  Discover what's new, Re-order your products with an amazing
                  Dashboard
                </h4>
                <p>
                  Trash the paper catalogues and know what your customers really
                  like, Keep track update and understand the customer using our
                  new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
        <div class="column is-4">
          <div data-aos="fade-left" class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fas fa-smile"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>
                  Discover what's new, Re-order your products with an amazing
                  Dashboard
                </h4>
                <p>
                  Trash the paper catalogues and know what your customers really
                  like, Keep track update and understand the customer using our
                  new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="intro column is-8 is-offset-2">
        <h2 class="title is-primary">
          Perfect for whole-salers, retailers and individuals!
        </h2>
        <br />
        <p class="subtitle">
          Request for a demo and save yourself some time doing inventory
          management and Logistics.
        </p>
      </div>
    </section>
    <br />
    <br />
    <br />
    <br />
    <br />
    <section class="container">
      <div data-aos="fade-right" class="intro column is-8 is-offset-2">
        <b-button
          class="button is-primary is-rounded"
          to="/sell"
          size="is-large"
          >Sell</b-button
        >
        <br />
        <br />
        <br />
        <p data-aos="fade-down" class="title">
          Start reaching out to your customers <br />and expand.⬆
        </p>
        <br />
      </div>
    </section>
    <section class="container">
      <div class="columns features">
        <div class="column is-4">
          <div data-aos="fade-right" class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fas fa-smile"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>
                  Discover what's new, Re-order your products with an amazing
                  Dashboard
                </h4>
                <p>
                  Trash the paper catalogues and know what your customers really
                  like, Keep track update and understand the customer using our
                  new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
        <div class="column is-4">
          <div data-aos="fade-up" class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fas fa-smile"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>
                  Discover what's new, Re-order your products with an amazing
                  Dashboard
                </h4>
                <p>
                  Trash the paper catalogues and know what your customers really
                  like, Keep track update and understand the customer using our
                  new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
        <div class="column is-4">
          <div data-aos="fade-left" class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fas fa-smile"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>
                  Discover what's new, Re-order your products with an amazing
                  Dashboard
                </h4>
                <p>
                  Trash the paper catalogues and know what your customers really
                  like, Keep track update and understand the customer using our
                  new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="hero is-medium has-text-centered">
      <div class="hero-body">
        <div class="container">
          <div class="columns is-centered">
            <div data-aos="zoom-in-up" class="column is-8">
              <!-- <h1 class="title titled is-1 mb-6">
                Primary bold title <span id="typewriter"></span>
              </h1>
              <h2 class="subtitle subtitled">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                Laborum cupiditate dolorum vitae dolores nesciunt totam magni
                quas. Lorem ipsum, dolor sit amet consectetur adipisicing elit.
              </h2> -->
              <h3 class="title titled is-1 mb-6">
                We would love to hear from you!<span id="typewriter"></span>
              </h3>
              <contactForm />
            </div>
          </div>
        </div>
      </div>
    </section>
    <transition
      enter-active-class="animate__animated animate__fadeInDown"
      leave-active-class="animate__animated animate__fadeOutUp"
    >
      <b-modal
        v-model="showRegister"
        has-modal-card
        trap-focus
        :destroy-on-hide="false"
        aria-role="dialog"
        aria-label="Example Modal"
        aria-modal
      >
        <template>
          <registerForm />
        </template>
      </b-modal>
    </transition>
    <transition
      enter-active-class="animate__animated animate__fadeInDown"
      leave-active-class="animate__animated animate__fadeOutUp"
    >
      <b-modal
        v-model="showLogin"
        :destroy-on-hide="false"
        aria-role="dialog"
        aria-label="Example Modal"
        aria-modal
      >
        <template>
          <loginForm />
        </template>
      </b-modal>
    </transition>
  </div>
</template>

<script>
import registerForm from "../components/registerForm.vue";
import loginForm from "../components/loginForm.vue";
import contactForm from "../components/ContactForm.vue";
// @ is an alias to /src

export default {
  name: "Home",
  data() {
    return {
      showLogin: false,
      showRegister: false
    }
  },
  components: {
    contactForm,
    registerForm,
    loginForm,
  },
};
</script>

<style>
.image {
  height: 100px;
}
.button {
  color: aqua;
}
</style>
