<template>
   <section id="details">
      <div class="details-img">
         <img src="/ice-cave.jpeg" />
         <div class="details-img-text">
            <strong>
               <i class="fas fa-map-marker-alt"></i>
               Iceland
            </strong>
            <small>Ice Caves</small>
            <small> $ {{ budget }}</small>
         </div>
      </div>
   </section>
</template>

<script>
   
   import { ref } from 'vue'
   
   export default {
      name: 'Details',
      setup() {
         
         const budget = ref(200)
         
         return { budget }
      }
   }
   
</script>

<style lang="scss" >
   
   @import './src/sass/_details';
   
</style>