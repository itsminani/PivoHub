<template>
  <div id="app">
    <div id="nav" v-if="$route.name != 'Admin'">
      <b-navbar spaced>
        <template #brand>
          <b-navbar-item tag="router-link" :to="{ path: '/' }">
            <img class="image" alt="logo" src="./assets/logo.png" />
          </b-navbar-item>
        </template>
        <template #start>
          <router-link to="/">
            <b-navbar-item to="/home">
              Home
            </b-navbar-item>
          </router-link>
          <router-link to="/about">
            <b-navbar-item to="/about">
              About
            </b-navbar-item>
          </router-link>
          <b-navbar-dropdown label="Info">
            <b-navbar-item href="#">
              About
            </b-navbar-item>
            <b-navbar-item href="#">
              Contact
            </b-navbar-item>
          </b-navbar-dropdown>
        </template>

        <template #end>
          <b-navbar-item tag="div">
            <div class="buttons">
              <a @click="showRegister = true" class="button is-primary">
                <strong>Sign up</strong>
              </a>
              <a @click="showLogin = true" class="button is-light">
                Log in
              </a>
            </div>
          </b-navbar-item>
        </template>
      </b-navbar>
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
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    </div>
    <div class="container-max-width">
      <div class="">
        <transition
          mode="out-in"
          enter-active-class="animate__animated animate__fadeIn"
          leave-active-class="animate__animated animate__fadeOut"
        >
          <router-view />
        </transition>
      </div>
    </div>
  </div>
</template>
<script>
AOS.init({
  once: false,
  mirror: true,
  duration: 600,
});
import registerForm from "./components/registerForm.vue";
import loginForm from "./components/loginForm.vue";
export default {
  data() {
    return {
      showRegister: false,
      showLogin: false,
      deferredPrompt: null
    };
  },
  methods: {
    async install() {
      this.deferredPrompt.prompt();
    },
    hasCancel() {
      this.$buefy.snackbar.open({
        indefinite: true,
        message: "This web-app can be installed too☺ by just clicking here",
        cancelText: "Cancel",
        onAction: () => {
          this.deferredPrompt.prompt();
          console.log("hello")
        },
      });
    },
  },
  created() {
    window.addEventListener("beforeinstallprompt", (e) => {
      e.preventDefault();
      // Stash the event so it can be triggered later.
      this.deferredPrompt = e;
    });
    window.addEventListener("appinstalled", () => {
      this.deferredPrompt = null;
    });
    if (this.deferredPrompt) {
      this.hasCancel();
    }
  },
  components: {
    registerForm,
    loginForm,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 0px;

  a {
    font-weight: bold;
    color: #2c3e50;
  }
}
</style>
