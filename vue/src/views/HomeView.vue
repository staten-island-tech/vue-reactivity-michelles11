import TheWelcome from '../components/TheWelcome.vue'
<template>
  <TheWelcome />
  <div class="home">
    <Button @button-click="bye">Button 1</Button>
    <Button @button-click="hello">Button 2</Button>
    <Card
      title="Hello World"
      description="blah blah blah "
      image="https://upload.wikimedia.org/wikipedia/commons/thumb/3/30/Vulpes_vulpes_ssp_fulvus.jpg/1200px-Vulpes_vulpes_ssp_fulvus.jpg"
    ></Card>
  </div>
</template>

<script>
import Button from '../components/Button.vue'
import Card from '../components/Card.vue'
export default {
  name: 'Home',
  components: {
    Button,
    Card
  },
  data() {
    return {
      tvshows: [
        'Gilmore Girls',
        'Friends',
        'The Office',
        'The Vampire Diaries',
        'How I Met Your Mother',
        'Breaking Bad',
        'Arrested Development',
        'Outer Banks',
        'Ted Lasso',
        'Shrinking',
        'A Series of Unfortunate Events',
        'Jane The Virgin',
        'Emily In Paris',
        'Gossip Girl',
        ''
      ]
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
