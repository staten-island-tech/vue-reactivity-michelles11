import TheWelcome from '../components/TheWelcome.vue'
<template>
  <TheWelcome />
  <div class="home">
    <select v-model="selected">
    <option value =""></option>
    </option></select>
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {},
  data() {
    return {
      checkedNames: []
    }
  },
  methods: {}
}
</script>

<style></style>
