import TheWelcome from '../components/TheWelcome.vue'
<template>
  <TheWelcome />
  <div class="home">
    <Button @button-click="bye">Button 1</Button>
    <Button @button-click="hello">Button 2</Button>
  </div>
</template>

<script>
import Button from '../components/Button.vue'
export default {
  name: 'Home',
  components: {
    Button
  },
  data() {
    return {
      selected: ''
    }
  },

  methods: {
    hello: function () {
      console.log('hello')
    },
    bye: function () {
      console.log('goodbye')
    }
  }
}
</script>

<style></style>
