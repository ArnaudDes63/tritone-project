<template>
  <div class="achats">
    <h1>Nos Articles</h1>

    <ma-card></ma-card>

     
    
   


  </div>
</template>

<script>
import MaCard from './Card/MaCard.vue'



export default {
  components: { MaCard },
  name: 'MaPageAchat',
   
}
</script>

<style  scoped>

*, ::before, ::after {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}

.achats{
  background: #333;    
}

h1{  
  margin: 90px;
  color:  #f1f1f1;
  text-align: center;
  font-size: 50px;  
}










</style>