import TheWelcome from '../components/TheWelcome.vue'
<template>
  <TheWelcome />
  <div class="home">
    <Button></Button>
  </div>
</template>

<script>
import Button from '../components/Button.vue';
export default {
  name: 'Home',
  components: {
    Button,
  },
  data() {
    return {
      selected: '',
    };
  }
  methods: {},
  }
</script>

<style></style>
