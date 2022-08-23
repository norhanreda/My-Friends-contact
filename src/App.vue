<template>
  <section>
    <h2>My friends</h2>
    
      <friend-contact> </friend-contact>
      <friend-contact> </friend-contact>
   
  </section>
</template>

<script>
import FriendContact from "./components/FriendContact.vue";

export default {
  data() {
    return {};
  },
  components: {
    FriendContact,
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
