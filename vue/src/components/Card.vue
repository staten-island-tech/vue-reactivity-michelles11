<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <img :src="image" alt="" />
    <h3>{{ streaming }}</h3>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    image: String,
    streaming: String
  }
}
</script>

<style>
.card {
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
/* .image {
  height: 50%;
  border-radius: 1rem;
} */
</style>
