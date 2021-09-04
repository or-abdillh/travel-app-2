<template>
   <section id="home">
      <Header></Header>
      <SearchBar></SearchBar>
      <Category></Category>
      <Nav></Nav>
      <div class="content">
         <div class="content-title">
            <strong>Recomended</strong>
            <small>see more</small>
         </div>
         <div class="content-card">
            <template v-for="card in 4" :key="card" >
               <Card></Card>
            </template>
         </div>
      </div>
   </section>
</template>

<script>
   
   import Header from '../components/Header.vue'
   import SearchBar from '../components/SearchBar.vue'
   import Category from '../components/Category.vue'
   import Nav from '../components/Nav.vue'
   import Card from '../components/Card.vue'
   
   export default {
      name: 'Home',
      components: {
         Header,
         SearchBar,
         Category,
         Nav,
         Card
      }
   }
</script>

<style lang="scss">
   
   @import './src/sass/_home'
   
</style>