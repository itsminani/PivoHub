<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h1 class="title titled is-1 mb-6">
      E-MarketPlace
    </h1>
    <p>
      This was made using Vue JS<br />
      check out the
      <a href="" target="_blank" rel="noopener"
        >Vue</a
      >.
    </p>
    <h3>Technologies used</h3>
    <ul>
      <li>
        <a
          href=""
          target="_blank"
          rel="noopener"
          >babel</a
        >
      </li>
      <li>
        <a
          href=""
          target="_blank"
          rel="noopener"
          >pwa</a
        >
      </li>
      <li>
        <a
          href=""
          target="_blank"
          rel="noopener"
          >router</a
        >
      </li>
      <li>
        <a
          href=""
          target="_blank"
          rel="noopener"
          >vuex</a
        >
      </li>
      <li>
        <a
          href=""
          target="_blank"
          rel="noopener"
          >eslint</a
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
