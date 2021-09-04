<template>
   <section class="search-bar">
      <div class="search-bar-wrapper">
         <span>
            <i class="fa fa-search" ></i>
         </span>
         <input type="text" placeholder="Search destination" />
      </div>
      <div class="search-bar-filter">
         <i class="fas fa-sliders-h"></i>
      </div>
   </section>
</template>

<script>
   
   export default {
      name: 'SearchBar'
   }
   
</script>

<style lang="scss" >
   
   @import './src/sass/_searchBar'
   
</style>