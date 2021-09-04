<template>
   <section class="nav">
      <template v-for="item in navs" :key="item.title">
         <div @click="navActive = item.title" :class="navActive == item.title ? 'active' : ''" class="nav-item">
            <i :class="item.icon" ></i>
            <span v-if="navActive == item.title" >{{ item.title }}</span>
         </div>
      </template>
   </section>
</template>

<script>
   
   import { ref } from 'vue'
   
   export default {
      name: 'Nav',
      setup() {
         
         const navs = ref([
            {title: 'Home', icon: 'fa fa-home'},
            {title: 'Search', icon: 'fa fa-search'},
            {title: 'Bookmark', icon: 'fa fa-bookmark'},
            {title: 'Profile', icon: 'fa fa-user'}
            ])
         
         const navActive = ref('Home')
            
         return { navs, navActive }   
      }
   }
   
</script>

<style lang="scss" >
   
   @import './src/sass/_nav';
   
</style>