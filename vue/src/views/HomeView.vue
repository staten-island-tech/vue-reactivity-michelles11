import TheWelcome from '../components/TheWelcome.vue'
<template>
  <main>
    <TheWelcome />
    <div class="home">
      <button v-if="loggedIn">Log Out</button>
      <button v-else>Login</button>
  </main>
</template>

<script>
export default {
  name: 'Home',
  components: {},
  data() {
    return {
      student: 'Harry',
      graduated: true,
      animals: ['Pig', 'Horse', 'Donkey', 'Cow', 'Duck']
      //animals
    }
  }
}
</script>
<style></style>
