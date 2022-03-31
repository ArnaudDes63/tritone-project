<template>
  <div id="app">
    <div class="MonHeader"><mon-header></mon-header></div>
    
    <router-view></router-view>
    
     <div class="Monfooter"><mon-footer></mon-footer></div>
   
  </div>
</template>

<script>



import MonFooter from './components/MonFooter.vue'
import MonHeader from './components/MonHeader.vue'






export default {
  name: 'App',
  components: {
    'MonFooter' : MonFooter,
    'MonHeader' : MonHeader
  }
  
  
  
}
</script>

<style>

#app{  
  max-height: 100vh;  
}

@media(max-height: 1200px){
  #app{
    max-height: 5vh;
}
}






</style>
