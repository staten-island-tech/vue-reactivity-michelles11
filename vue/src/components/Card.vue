<template>
  <div class="card">
    <h2>{{ title }}</h2>
    <img :src="getImage" alt="" />
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
  },
  computed: {
    getImage: function () {
      return this.image
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
</style>
