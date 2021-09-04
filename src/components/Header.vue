<template>
   <div class="header">
      <div class="header-profile">
         <span class="profile-img">
            <i class="fas fa-user-alt"></i>
         </span>
         <div class="profile-wellcome">
            <small>Hello there,</small>
            <strong>Daniel</strong>
         </div>
      </div>
      <span class="header-bell">
         <i class="fas fa-bell"></i>
      </span>
   </div>
</template>

<script>
   
   export default {
      name: 'Header'
   }
   
</script>

<style lang="scss">
   
   @import './src/sass/_header'
   
</style>