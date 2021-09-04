<template>
   <section id="home">
      <Header></Header>
      <SearchBar></SearchBar>
      <Category></Category>
   </section>
</template>

<script>
   
   import Header from '../components/Header.vue'
   import SearchBar from '../components/SearchBar.vue'
   import Category from '../components/Category.vue'
   
   export default {
      name: 'Home',
      components: {
         Header,
         SearchBar,
         Category
      }
   }
</script>

<style lang="scss">
   
   @import './src/sass/_home'
   
</style>