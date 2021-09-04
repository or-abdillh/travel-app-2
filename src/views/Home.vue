<template>
   <section id="home">
      <Header></Header>
   </section>
</template>

<script>
   
   import Header from '../components/Header.vue'
   
   export default {
      name: 'Home',
      components: {
         Header
      },
      setup() {
         
      }
   }
</script>

<style lang="scss">
   
   @import './src/sass/_home'
   
</style>