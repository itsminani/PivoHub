<template>
  <div class="about">
    <section class="hero mainBack is-large is-bold">
      <div class="hero-head">
        <!-- <nav class="navbar">
          <div class="container">
            <div class="navbar-brand">
              <a class="navbar-item" href="../">
                <img
                  src="http://bulma.io/images/bulma-type-white.png"
                  alt="Logo"
                />
              </a>
              <span class="navbar-burger burger" data-target="navbarMenu">
                <span></span>
                <span></span>
                <span></span>
              </span>
            </div>
            <div id="navbarMenu" class="navbar-menu">
              <div class="navbar-end">
                <div class="tabs is-right">
                  <ul>
                    <li class="is-active"><a>Home</a></li>
                    <li><a href="">Examples</a></li>
                    <li><a href="">Features</a></li>
                    <li><a href="">Team</a></li>
                    <li><a href="">Help</a></li>
                  </ul>
                  <span class="navbar-item">
                    <a
                      class="button is-white is-outlined"
                      href="https://github.com/BulmaTemplates/bulma-templates/blob/master/templates/hero.html"
                    >
                      <span class="icon">
                        <i class="fa fa-github"></i>
                      </span>
                      <span title="Hello from the other side">View Source</span>
                    </a>
                  </span>
                </div>
              </div>
            </div>
          </div>
        </nav> -->
      </div>
      <div class="hero-body">
        <div class="container has-text-centered">
          <h1 class="title">
            Buy & Sell Craft Beverages The Easy Way
          </h1>
          <h2 class="subtitle">
            PivoHub streamlines and grows your business. Whether you're a buyer,
            producer, or distributor, <br> our tools ease the pain of daily manual
            tasks and put the focus back on sales.
          </h2>
        </div>
      </div>
    </section>
    <div class="box cta">
      <p class="has-text-centered">
        <span class="tag is-primary">New</span> This Part Will include all the
        news about the company and upcoming changes
      </p>
    </div>
    <div class="intro column is-8 is-offset-2">
      <b-button class="button is-primary is-rounded" to="/buy" size="is-large"
        >Buy</b-button
      >
      <br />
      <br>
      <br>
      <p class="title">Order anytime, anywhere... <br />Even on the 🚽😂</p>
      <br>
    </div>
    <section data-aos="fade-up" class="container">
      <div class="columns features">
        <div class="column is-4">
          <div class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fa fa-paw"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>Discover what's new, Re-order your products with an amazing Dashboard</h4>
                <p>
                  Trash the paper catalogues and know what your customers really like, Keep track update and understand the customer using our new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
        <div class="column is-4">
          <div class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fa fa-empire"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>Discover what's new, Re-order your products with an amazing Dashboard</h4>
                <p>
                  Trash the paper catalogues and know what your customers really like, Keep track update and understand the customer using our new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
        <div class="column is-4">
          <div class="card is-shady">
            <div class="card-image has-text-centered">
              <i class="fa fa-apple"></i>
            </div>
            <div class="card-content">
              <div class="content">
                <h4>Discover what's new, Re-order your products with an amazing Dashboard</h4>
                <p>
                  Trash the paper catalogues and know what your customers really like, Keep track update and understand the customer using our new analytics software.
                </p>
                <p><a href="#">Learn more</a></p>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="intro column is-8 is-offset-2">
        <h2 class="title is-primary">Perfect for whole-salers, retailers and individuals!</h2>
        <br />
        <p class="subtitle">
          Request for a demo and save yourself some time doing inventory management and Logistics.
        </p>
      </div>
    </section>
    <footer class="footer">
      <div class="container">
        
          <div class="control level-item">
              <div class="tags has-addons">
                <span class="tag is-info">Made Using Vue + Javascript + AWS</span>
              </div>
            </a>
          </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>

<style>
.mainBack {
  background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
  background-size: 400% 400%;
  animation: gradient 15s ease infinite;
  height: 100vh;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
</style>
