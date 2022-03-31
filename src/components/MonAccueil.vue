<template>
 

  <section class="hero" >

    <div class="card">
      <h1>Bienvenue Sur triTone</h1>
      <span>RETRO</span>
      <img class="saxo" src="../assets/saxophone.svg" alt="">
    </div>

    

    <ma-modale :revele="revele" :toggleModale="toggleModale"></ma-modale>

    <div v-on:click="toggleModale" class="btn btn-danger">Ouvrir La Vidéo D'Intro</div>

     <img class="logo" src="../assets/logo.svg" alt="Ici ce trouve le Logo du site tritone">




  </section>
</template>

<script>

import MaModale from './MaModale.vue'

export default {
    name: 'MonAccueil',
    components: {MaModale},
    data(){
      return {
        revele: false        
        }
      },
      methods: {
        toggleModale : function(){
          this.revele = !this.revele
        }
      }

}
</script>

<style scoped>

*, ::before, ::after{
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}


.hero{  
  
  width: 100%;
  height:100vh;  
  background: linear-gradient(rgba(0, 0, 0, 0.555), transparent), url('../assets/background.jpeg');
  background-size: cover; 
  background-position:20%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}



img{
  position: fixed;
  right: 0; 
  bottom: 1%;
  width: 100px;
  height: 250px;
}

.btn{
  position: fixed;
  font-weight: bold;  
  color: #FFFFFF !important;
  font-size: 20px;
  text-shadow: 2px 3px 1px #FF2EFF;
  box-shadow: 4px 3px 5px #B00E90;
  padding: 0px ;
  border-radius: 10px;
  border: 2px solid #3866A3;
  background: #EE0505;
  top: 110px;
  width: 40%;  
}

.btn:hover {
  color: #FFFFFF !important;
  background: #000000;
}

.card {
  background: none;
    width: 850px;
    position: absolute;
    top: 55%;
    left: 50%;
    transform: translate(-50%, -50%);
    padding: 50px 80px 120px;
    box-shadow:
    0 0 10vw  0vw rgb(170, 15, 231),   
    0 0   2vw  0.4vw rgb(170, 15, 231),
    
    inset 0 0 .5vw  .2vw rgb(170, 15, 231),
    inset 0 0 0.2vw  0.2vw rgb(170, 15, 231),
    inset 0 0 .25vw  0.2vw rgb(170, 15, 231);
    border-radius: 22px;
}

.card h1 {
    
    font-size: 36px;
    font-weight: 300;
    color: #ffffffe3;
    text-shadow:
    .1vw 0vw .25vw rgb(170, 15, 231), 
    .15vw 0vw .25vw rgb(170, 15, 231), 


    .1vw 0vw  .1vw #3134ff, 
    .15vw 0vw  .1vw #3134ff, 
    .4vw 0vw  .1vw #3134ff,

    .1vw 0vw   2vw #3134ff, 
    .15vw 0vw   2vw #3134ff, 
    .4vw 0vw   2vw #3134ff, 

    .1vw 0vw   1vw #0408fb, 
    .15vw 0vw   1vw #0408fb, 
    .4vw 0vw   5vw #0408fb, 

    .1vw 0vw   5vw #0408fb, 
    .15vw 0vw  20vw #0408fb, 
    .4vw 0vw  10vw #0408fb,
    
    .1vw 0vw  10vw #0408fb, 
    .15vw 0vw  30vw #0408fb, 
    .4vw 0vw  10vw #0408fb;

    animation: blink 2s infinite alternate;
}


.card span {
    
    padding-left: 10px;
    padding-top: 15px;
    font-size: 35px;
    letter-spacing: 5px;
    color: #ffffffcb;
    text-shadow:
    .1vw 0vw .25vw #ff7474, 
    .125vw 0vw .25vw #ff7474, 

    .1vw 0vw  .1vw #ff3131, 
    .125vw 0vw  .1vw #ff3131, 
    .15vw 0vw  .1vw #ff3131,

    .1vw 0vw   2vw #ff3131, 
    .125vw 0vw   2vw #ff3131, 
    .15vw 0vw   2vw #ff3131, 

    .1vw 0vw   1vw #fb0404, 
    .125vw 0vw   1vw #fb0404, 
    .15vw 0vw   5vw #fb0404, 

    .1vw 0vw   5vw #fb0404, 
    .125vw 0vw  20vw #fb0404, 
    .15vw 0vw  10vw #fb0404;

}

.card img {
    position: absolute;
    width: 200px;
    filter: 
    drop-shadow(0 0.15vw 0.30vw #fffb0e)
    drop-shadow(0 0.15vw 0.30vw #8a8942);
    animation: saxo-blink 2s infinite alternate;  
}



@keyframes blink {
    
    0%, 18%, 22%, 25%, 53%, 57%, 100% {
  
        text-shadow:
        0 0   0.5vw #7476ff,
        0.1vw 0 0.5vw #7476ff,
        0.3vw 0 0.5vw #7476ff,
    
        0 0 1.2vw #3134ff,
        0.1vw 0 1.2vw #3134ff,
        0.3vw 0 1.2vw #3134ff,
    
    
        0 0 3vw #0408fb,
        0.1vw 0 3vw #0408fb,
        0.3vw 0 3vw #0408fb;
    
    }
    
    20%, 24%, 55% {        
        text-shadow: none;
    }    
  }
  
  @keyframes saxo-blink {
    0%, 9%, 15%, 79%, 83%, 100%{
  
        filter: 
        drop-shadow(0 0.15vw 0.30vw #fffb0e)
        drop-shadow(0 0.15vw 0.30vw #8a8942);
    
    }
    
    10%, 14%, 80%, 82% {        
        
        filter: none;
    }
  }

@media(max-width:850px) {
  .card{
    width: 500px;
  }
  .card h1{
    font-size: 21px;    
  }
  .card span{
    font-size: 22px;    
  }
  .card img{
    width: 130px;
  }
  .btn{
    width: 40%
  }
}

@media (max-width : 501px){
  .card{
    width: 350px;
  }
  .card h1{
    font-size: 15px;    
    margin-left: -60px;
  }
  .card img{
    width: 120px;
  }

  .logo{
    width: 150px;
    margin: 5px;
    padding-top: 30px;
  }

  .btn{
    width: 150px
  }

  .logo{  
        display: block;
        visibility: hidden;       
    }
}

</style>