<template>
  <div>
    <h1 class="homestyle">Hello from Home Component</h1>
    <h1 v-bind:style="{color: 'blue' }">Style binding</h1>
    <h1 v-bind:class="{display:show}">Class binding</h1>
    <h1 v-bind:class="[aclass]"> Array binding</h1>
    
  </div>
</template>

<script>
export default {
  name: "New",
  data(){
    return{
      show: true,
      aclass: "array"
    }
  }
 
  
}
</script>

<style scoped>
.homestyle{
  color: rgb(255, 153, 0);
}
.display{
  background-color: burlywood;
}
.array{
  background-color: rgb(127, 243, 243);
}
</style>