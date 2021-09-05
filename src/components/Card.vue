<template>
   <div class="card-wrapper">
      <img src="/ice-cave.jpeg" />
      <span class="card-bookmark" >
         <i class="fa fa-bookmark" ></i>
      </span>
      <div class="card-content">
         <strong @click="$router.push({name: 'Details'})" >Ice Caves</strong>
         <small>
            <i class="fas fa-map-marker-alt"></i>
            Iceland
         </small>
         <small>
            Starting at
            <span>$200</span>
         </small>
      </div>
   </div>
</template>

<script>
   
   export default {
      name: 'Card'
   }
   
</script>

<style lang="scss" >
   
   @import './src/sass/_card';
   
</style>