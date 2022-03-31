<template>
  <div class="navbar fixed-top navbar-expand-lg navbar-dark">
      <div class="has-bg-img">
          <img class="bg-img"  src="../assets/triTone.png" >
          <div></div>
          <p>Virtual Instrument Engine</p>
      </div>      
  </div>
</template>

<script >
export default {
    name: 'MonHeader'

}
</script>

<style scoped>



.navbar{    
    position: fixed;
    background: rgb(202, 27, 27);
    height: 90px;
    width: 100%;
}

img.bg-img{
    display: block;
    position: absolute;
    width: 450px;
    max-height: 150px;   
    top: -20px;
}

p{
    font-family: 'Kosugi Maru', sans-serif;
    display: block;
    justify-content: center;
    align-content: center;
    position: absolute;
    font-size: 2em;
    right: 100px;
    top: 10px;
    color: white;
    
    
}

@media screen and (max-width: 925px) {
	img.bg-img{
        
        width: 300px;
        top: -10px;
    }
    p{
        font-size: 2rem;
        padding: 10px;
        margin-right: -80px;
    }
    
}

@media(max-width:768px) {
    img.bg-img{
        
        width:250px;
        top: 10px;	
    }
    
    p {
		font-size: 1.2em;
        padding: 20px;
        margin-right: -100px;
        
	}
}

@media(max-width:500px) {
        
    p {
		font-size: 1em;
        padding: 5px;
        margin-right: -100px;
        
	}
}


</style>