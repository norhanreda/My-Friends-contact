<template>
  <li>
    <h2>{{ firend.name }}</h2>
    <button @click="toggleDetails">
      {{ DetailsAreVisable ? "Hide" : "Show" }} Details
    </button>
    <ul>
      <li>
        <strong>Phone: </strong>
        {{ firend.phone }}
      </li>
      <li>
        <strong>E-mail:</strong>
        {{ firend.emial }}
      </li>
    </ul>
  </li>
</template>

<script>
export default {
  data() {
    return {
      firend: {
        id: "5",
        name: "norhan",
        phone: "01003874842",
        emial: "norhanreda12345@gmail.com",
        DetailsAreVisable: "true",
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
