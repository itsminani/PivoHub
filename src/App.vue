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
          <b-navbar-dropdown label="User">
            <b-navbar-item @click="showRegister = true" href="#">
              Account
            </b-navbar-item>
            <router-link to="/admin">
              <b-navbar-item>
                Admin Demo
              </b-navbar-item>
            </router-link>
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
              <a
                @click="install()"
                v-if="deferredPrompt"
                class="button is-centered is-success is-rounded"
              >
                <i class="fas fa-download"></i> Install
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
    <b-navbar>
      <template #brand>
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img class="image" alt="logo" src="./assets/logo.png" />
        </b-navbar-item>
      </template>
      <template #start>
          <b-navbar-item class="animate" href="https://github.com/itsminani/PivoHub">
            This was made using &nbsp
            <b-tag type="is-success"> <span class="icon">
                  <i class="fab fa-vuejs"></i>
                </span> Vue Js</b-tag> &nbsp
            <b-tag type="is-warning"> <span class="icon">
                  <i class="fab fa-aws"></i>
                </span> AWS</b-tag> &nbsp
            <b-tag type="is-link"> <span class="icon">
                  <i class="fab fa-js-square"></i>
                </span> JS & TS</b-tag> &nbsp
            <b-tag type="is-dark"> <span class="icon"> 
                  <i class="fab fa-github"></i>
                </span> Github</b-tag>
          </b-navbar-item>
      </template>

      <template #end>
        <b-navbar-item tag="div">
          <div class="buttons">
            <a href="https://github.com/itsminani" class="button is-dark is-outlined">
              <span class="icon"> 
                  <i class="fab fa-github"></i>
                </span><strong>My Git</strong>
            </a>
            <a href="https://www.linkedin.com/in/heritierlucminani/" class="button is-link">
              <span class="icon"> 
                  <i class="fab fa-linkedin"></i>
                </span>My LinkedIn
            </a>
          </div>
        </b-navbar-item>
      </template>
    </b-navbar>
  </div>
</template>

<script>
AOS.init({
  once: false,
  mirror: true,
  duration: 600,
});
document.title = "PivoHub";
import registerForm from "./components/registerForm.vue";
import loginForm from "./components/loginForm.vue";
export default {
  data() {
    return {
      showRegister: false,
      showLogin: false,
      deferredPrompt: null,
    };
  },
  methods: {
    async install() {
      this.deferredPrompt.prompt();
    },
    pause() {
      this.$buefy.toast.open({
        duration: 5000,
        message: `This is still <b>in development</b>, The text is <br/> just placeholder text that I found on your website.
        <br/> The functionality doesn't work. I am Currently working on adding an <b>AWS Backend</b>`,
        type: "is-success",
        position: "is-bottom",
        pauseOnHover: true,
      });
    },
  },
  created() {
    this.pause();
    window.addEventListener("beforeinstallprompt", (e) => {
      e.preventDefault();
      // Stash the event so it can be triggered later.
      this.deferredPrompt = e;
    });
    window.addEventListener("appinstalled", () => {
      this.deferredPrompt = null;
    });
    if (this.deferredPrompt) {
      console.log("I am Finally working");
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
.animate{
  animation-duration: 1s;
  transition: 0.3s;
}
.animate:hover{
  transform: scale(1.02);
  transition: 0.3s;
}
</style>
