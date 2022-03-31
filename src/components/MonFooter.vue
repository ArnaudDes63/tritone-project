<!-- Ici ce trouver mon component pour les liens de la page ( Footer ) -->
<template>
<header class="header">
    <nav>

       <ul>
    
       <div class="item">  <router-link to="/" exact>Acceuil</router-link></div>
       <div class="item">  <router-link to="/MaPageContact">Contact</router-link></div>
       <div class="item">  <router-link to="/MaPageAchat">Achat</router-link></div>
       <div class="item">  <router-link to="/MaPageProduit">Produit</router-link></div>

       </ul>
    
    </nav>
    
</header>


  
</template>



<script>





export default {
    name: 'MonFooter',
    }
   


</script>



<style scoped>

*, ::before, ::after {
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
    overflow-x: hidden;    
}

.header{
    position: fixed;    
    bottom: 0;
    height: 80px;
    background: rgb(202, 27, 27);
    width: 100%;        
    font-size: 20px;
    display: flex;
    justify-content: space-around;
    
}

a{
    color: #fff;
    text-decoration: none;    
    font-size: 1.2rem;
    display: block;
    
} 

a:hover {
     color: rgb(0, 0, 0);    
     box-shadow: 10px 0 10px rgb(255, 255, 255);
     font-size: 21px;      
}

nav{
    min-height: 5vh;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;       
    margin: 1rem;
}  
nav ul{
    
    display: flex;
    flex: 1;
    justify-content: space-between;
    align-items: center;
    width: 50px;
    
    
}



/*  Header */

/* .main-head{
    position: fixed;       
    background: rgb(202, 27, 27);
    color: #fff;    
}

nav{
    min-height: 5vh;
    display: flex;
    align-items: center;
    width: 90%;
    margin: auto;
    padding: 1rem;
}

nav ul{
    
    display: flex;
    flex: 1;
    justify-content: space-between;
    align-items: center;
    width: 50px;
    
    
}
a:hover {
     color: rgb(0, 0, 0);    
     box-shadow: 10px 0 10px rgb(255, 255, 255);
     font-size: 21px;      
}  */


</style>