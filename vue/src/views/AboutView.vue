<template>
  <div class="My Cart"></div>
  <Card v-for="items in store" :key="items.name" :title="items.name" :image="items.imag" />
</template>
<script>
import Card from '../components/Card.vue'
import { store } from '../components/store.js'
export default {
  data() {
    return {
      store
    }
  },
  components: {
    Card
  }
}
</script>
<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
