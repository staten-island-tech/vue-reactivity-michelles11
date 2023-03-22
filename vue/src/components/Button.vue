<template>
  <button @click="$emit('button-click')"><slot></slot></button>
</template>

<script>
export default {
  name: 'Button'
}
</script>

<style scoped>
button {
  width: 200px;
  font-size: 30px;
  border-radius: 20px;
  border: none;
  background-color: red;
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
