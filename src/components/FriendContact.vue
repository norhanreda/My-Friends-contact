<template>
  <li>
    <h2>{{ name }}</h2>
    <button @click="toggleDetails()">
      {{ DetailsAreVisable ? "Hide" : "Show" }} Details
    </button>
    <ul v-if="DetailsAreVisable">
      <li>
        <strong>Phone: </strong>
        {{ phoneNumber }}
      </li>
      <li>
        <strong>E-mail:</strong>
        {{ emailAddress }}
      </li>
    </ul>
  </li>
</template>

<script>
export default {
  props:[
  'name',
  'phoneNumber',
  'emailAddress',

  ],
  data() {
    return {
      DetailsAreVisable: false,
      firend: {
        id: "5",
        name: "norhan",
        phone: "01003874842",
        emial: "norhanreda12345@gmail.com",
        
      },
    };
  },
  methods: {
    toggleDetails() {
      this.DetailsAreVisable = !this.DetailsAreVisable;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
