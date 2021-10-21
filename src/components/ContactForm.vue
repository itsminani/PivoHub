<template>
  <div class="box is-grey" >
    <section>
      <b-field horizontal label="Subject" message="Please enter a subject">
        <b-input name="subject" v-model="subject" expanded></b-input>
      </b-field>

      <b-field horizontal label="From">
        <b-input
          name="name"
          placeholder="Name"
          v-model="name"
          expanded
        ></b-input>
        <b-input
          name="email"
          type="email"
          v-model="email"
          placeholder="nobody@nowhere.com"
          expanded
        ></b-input>
      </b-field>

      <!-- <b-field horizontal label="Topic">
      <b-select placeholder="Select a topic">
        <option value="1">Bulma</option>
        <option value="2">Vue.js</option>
        <option value="3">Buefy</option>
      </b-select>
    </b-field> -->

      <b-field horizontal label="Message">
        <b-input v-model="message" type="textarea"></b-input>
      </b-field>

      <b-field horizontal
        ><!-- Label left empty for spacing -->
        <p class="control">
          <b-button @click="submit()" label="Send message" type="is-primary" />
        </p>
      </b-field>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      subject: "",
      email: "",
      message: "",
      name: "",
    };
  },
  methods: {
    submit() {},
  },
};
</script>