<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <img :src="getImage" alt="" />
    <h3>{{ streaming }}</h3>
    <button @click="Addtocart">Add to Cart</button>
  </div>
</template>
<script setup>
import { store } from './store.js'
</script>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    image: String,
    streaming: String
  },
  computed: {
    getImage: function () {
      return this.image
    }
  },
  methods: {
    Addtocart: function () {
      store.push({
        name: this.title,
        imag: this.getImage
      })
    }
  }
}
</script>

<style scoped>
.card {
  padding: 10px;
  text-align: center;
  border-radius: 25px;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: antiquewhite;
  width: 30%;
  height: 200px;
  margin: 10px auto;
}
img {
  border-radius: 1rem;
  height: 70%;
}
button {
  width: 100px;
  font-size: 20px;
  border-radius: 10px;
  border: none;
  background-color: #ac7165;
  color: white;
  transition: 0.3s;
}
button:hover {
  transform: scale(1.1);
}
button:active {
  transform: scale(0.6);
}
</style>
