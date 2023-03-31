<template>
  <div class="My Cart">
    <h1></h1>
  </div>
  <div>
    <button @click="store.increment()">From AboutView: {{ store.count }}</button>
  </div>
</template>
<script>
import { store } from '../store'
export default {
  data() {
    return {
      store
    }
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
