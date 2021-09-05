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
      <div class="details-content">
         <strong>About the destination</strong>
         <p>Start on adventure with a 3-days journey in Iceland and explore the caves</p>
         
         <div class="details-content-action">
            <div class="length">
               <span>
                  <i class="fa fa-clock" ></i>
                  Length
               </span>
               <span>
                  14 days
               </span>
            </div>
            <div class="person">
               <span>
                  <i class="fa fa-user" ></i>
                  Persons
               </span>
               <span>
                  <button @click="person++" type="button">+</button>
                  <p>{{ person }}</p>
                  <button :disabled="person == 0" @click="person--" type="button">-</button>
               </span>
            </div>
         </div>
         <div class="thumb-users">
            <template v-for="thumb in 5" :key="thumb" >
               <img src="/ice-cave.jpeg" class="thumb" />
               <div v-if="thumb == 5" class="thumb">
                  <strong>23+</strong>
               </div>
            </template>
         </div>
      </div>
      <div class="call-action">
         <span>
            <p>${{ budget * person }}</p>
            <p>({{ person }} tickets)</p>
         </span>
         <button type="button">
            Book now
         </button>
      </div>
   </section>
</template>

<script>
   
   import { ref, watch } from 'vue'
   
   export default {
      name: 'Details',
      setup() {
         
         const person = ref(1)
         const budget = ref(200)
         
         watch(person, () => {
            budget.value = person.value * 100
         })
         
         return { budget, person }
      }
   }
   
</script>

<style lang="scss" >
   
   @import './src/sass/_details';
   
</style>