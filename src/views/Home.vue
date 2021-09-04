<template>
   <section id="home">
      <Header></Header>
      <SearchBar></SearchBar>
      <Category></Category>
      <Nav></Nav>
   </section>
</template>

<script>
   
   import Header from '../components/Header.vue'
   import SearchBar from '../components/SearchBar.vue'
   import Category from '../components/Category.vue'
   import Nav from '../components/Nav.vue'
   
   export default {
      name: 'Home',
      components: {
         Header,
         SearchBar,
         Category,
         Nav
      }
   }
</script>

<style lang="scss">
   
   @import './src/sass/_home'
   
</style>