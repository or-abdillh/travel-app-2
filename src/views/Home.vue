<template>
   <section id="home">
      <Header></Header>
      <SearchBar></SearchBar>
   </section>
</template>

<script>
   
   import Header from '../components/Header.vue'
   import SearchBar from '../components/SearchBar.vue'
   
   export default {
      name: 'Home',
      components: {
         Header,
         SearchBar
      },
      setup() {
         
      }
   }
</script>

<style lang="scss">
   
   @import './src/sass/_home'
   
</style>