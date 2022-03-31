<template>
 <div class="galerie">

  

   <div class="item"><img src="https://cdn.pixabay.com/photo/2016/10/12/23/22/electric-guitar-1736291__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>
   </div>
   <div class="item"><img src="https://cdn.pixabay.com/photo/2016/08/15/16/48/vinyl-1595847__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>
   </div>
   <div class="item"><img src="https://cdn.pixabay.com/photo/2010/12/13/10/01/guitar-2119__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>
   </div>
   <div class="item"><img src="https://cdn.pixabay.com/photo/2016/11/29/09/08/headphones-1868612__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>
   </div>

   <div class="item"><img src="https://cdn.pixabay.com/photo/2020/04/15/14/45/microphone-5046876__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>
   </div>
   <div class="item"><img src="https://cdn.pixabay.com/photo/2016/11/21/11/32/audio-1844798__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>                              
   </div>
   <div class="item"><img src="https://cdn.pixabay.com/photo/2019/12/18/04/11/dj-4702977__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>             
   </div>
   <div class="item"><img src="https://cdn.pixabay.com/photo/2016/11/23/00/43/audio-1851517__340.jpg" alt="">
                  <div class="lien"><router-link to="/" exact>Acceuil🎬</router-link></div>
   </div>

   
   
 </div>
</template>



<script>

export default {
    name: 'MaCard',
    

}
</script>

<style lang="scss" scoped>

.galerie{  
  
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: flex-start;
  align-content: flex-start;
  height: 75vh; 
  max-width: 1900px;
  margin: 70px  auto;  
}



.item{
  
  width: 300px;
  height: 200px;
  margin: 12.5px;
  overflow: hidden;
  flex-shrink: 0;
}

.item img {
  
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.lien{
    color: #fff;
    position: absolute;
    display: flex;
    justify-content: center;
    text-decoration: none;
    width: 100px;
    height: 100px;
    padding: auto;
    
} 


@media(max-width: 1300px) {
  .galerie{
    height: 110vh;
  }
}

@media(max-width: 975px) {
  .galerie{
    height: 150vh;
    margin: 70px  auto;
  }
}

@media(max-width: 649px) {
  .galerie{
    height: 300vh;
    margin: 70px  auto;
  }
}


</style>