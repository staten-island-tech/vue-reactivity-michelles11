
<template>
  <h1>{{ student }}</h1>
</template>
<ul> 
<li v-for="animal in animals" :key="animal">{{ animal }}</li>
</ul>
</template>
</script>
export default {
  data(){
    return {
      student: "Jason",
      animals:["pig, "cow", "ostrich", "Zee"]
    }
  }
}