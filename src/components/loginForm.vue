<template>
  <div>
    <section class="hero is-white">
      <div class="hero-body">
        <div class="container has-text-centered ">
          <div class="">
            <h3 class="title has-text-primary">Login</h3>
            <hr class="login-hr" />
            <p class="subtitle has-text-black">Please login to proceed.</p>
            <div class="box">
              <form>
                <div class="field">
                  <div class="control">
                    <input
                      class="input is-large"
                      type="email"
                      placeholder="Your Email"
                      autofocus=""
                    />
                  </div>
                </div>

                <div class="field">
                  <div class="control">
                    <input
                      class="input is-large"
                      type="password"
                      placeholder="Your Password"
                    />
                  </div>
                </div>
                <div class="field">
                  <label class="checkbox">
                    <input type="checkbox" />
                    Remember me
                  </label>
                </div>
                <button class="button is-block is-primary is-large is-fullwidth">
                  Login <i class="fa fa-sign-in" aria-hidden="true"></i>
                </button>
              </form>
            </div>
            <p class="has-text-grey">
              <a href="../">Sign Up</a> &nbsp;·&nbsp;
              <a href="../">Forgot Password</a> &nbsp;·&nbsp;
              <a href="../">Need Help?</a>
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
    };
  },
};
</script>

<style>
hero {
  max-width: 100px;
}
</style>