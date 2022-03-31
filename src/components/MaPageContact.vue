<template>
<div class="container">

    <div class="item"><!-- Default form contact -->
<form class="text-center p-5" action="#!">

    <p class="h2 mb-4">Nous Contactez</p>

    <!-- Name -->
    <input type="text" id="defaultContactFormName" class="form-control mb-5" placeholder="Nom / Prénom">
    <input type="text" id="defaultContactFormName" class="form-control mb-5" placeholder="Entreprise / Particulier">
    <input type="text" id="defaultContactFormName" class="form-control mb-5" placeholder="TéLéphone">

    <!-- Email -->
    <input type="email" id="defaultContactFormEmail" class="form-control mb-5" placeholder="E-mail">

   

    <!-- Message -->
    <div class="form-group">
        <textarea class="form-control rounded-0" id="exampleFormControlTextarea2" rows="3" placeholder="Message"></textarea>
    </div>
    

    <!-- Send button -->
    <button class="btn btn-danger btn-block mt-2 p-2" type="submit">Envoyer</button>

</form>
<!-- Default form contact --></div>

    <div class="items"> <img src="../assets/shout.jpg" alt="Photo garçon avec un micro"/> </div>
    
   







</div>


</template>

<script>



export default {
    name: 'MaPageContact',
   

}
</script>

<style scoped>
/* Rezet */

*{
  margin: 15px;
  padding: 0;
  height: auto;
  width: 97%;

    
}

div{    
    max-width: 100%;      
    background-color: rgba(241, 228, 228, 0.233);    
}

.container{       
    
    display: flex;
    justify-content: center;      
}

.item{         
    width: 90%;
    height: 110vh;
    display: flex;
      
}

img{
    position: fixed;
    width: 50%;
    height: 100%;
    
    
    
}

.form-control,.browser-default{
    border: 2px solid rgb(0, 0, 0);
    text-align: center;   
    height: 6vh;    
}

.form-group{
    margin: 0px;
}

label{
    font-size: 1.3rem;
    margin: 10px;
     
}

.text-center{
    color: rgb(0, 0, 0);
}

.btn{
    display: block;
    width: 70%;
    height: 60px;
    border: 1px solid black;
    background-color: rgba(224, 71, 71, 0.836);
    font-size: 18px;
    color: white;
    outline: none;
    transition: 0.3s linear;
    margin: auto;
}

.btn:hover {
  transform: rotateY(35deg);
  box-shadow: -15px 0 15px rgb(0, 0, 0);
}



@media (max-width : 668px){
    img{
        display: block;
        visibility: hidden;       
    } 
     
    .form-control, .browser-default {
    
        position: relative;     
        width: 300px; 
        height: 6vh;  
        
        
        background: rgb(255, 255, 255);
        border: 2px solid rgb(0, 0, 0);
        color: black;        
    }

    .h2{ 
        position: relative; 
        right: 50px;
        width: 375px; 
        margin: 30px;   
          
    }
    
    .btn{
        position: relative;
        display: block;
        width: 200px;
        top: 10px;
        margin: 60px;
        
        }
        
}



</style>