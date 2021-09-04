<template>
   <section class="category">
      <template v-for="item in categories" :key="item" >
         <span @click="badgeActive = item" :class="badgeActive == item ? 'active' : ''" class="category-badge">
            {{ item }}
         </span>
      </template>
   </section>
</template>

<script>
   import { ref } from 'vue'
   
   export default {
      name: "Category",
      setup() {
         
         const categories = ref(['All', 'Adventures', 'Caves', 'Holidays'])
         const badgeActive = ref('All')
         
         return { categories, badgeActive }
      }
   }
   
</script>

<style lang="scss" >
   
   @import './src/sass/_category';
   
</style>