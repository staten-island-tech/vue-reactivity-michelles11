<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <img v-bind:src="image" alt="" />
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    description: String,
    image: String
  }
}
</script>

<style>
.card {
  width: 200px;
  padding: 10px;
  text-align: center;
  border-radius: 25px;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: antiquewhite;
  height: 500px;
  margin: 10px auto;
}
.image {
  height: 30vh;
  border-radius: 1rem;
}
</style>
