<template>
  <section>
    <h2 id="logo">My friends</h2>

    <friend-contact
      name="norhan reda"
      phone-number="01003874842"
      email-address="norhanreda12345@gmail.com"
    >
    </friend-contact>
    <friend-contact
      name="nono"
      phone-number="01003856656"
      email-address="nono@gmail.com"
    >
    </friend-contact>
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

#app #logo
{
background-color: palevioletred;
padding: 1rem;
margin: 1rem;
border-color: black ;

}
</style>
