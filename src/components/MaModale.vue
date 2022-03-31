<template>

    <div class="bloc-modale" v-if="revele">

            <div v-on:click="toggleModale" class="overlay"></div>

                <div class="modale card">
                    
                    
                    <video ref="videoRef" src="../assets/Video_accueil.mp4" id="video-container" width="350px" height="200px" controls></video>
                    
                    <div v-on:click="toggleModale" class="btn-modale btn btn-danger">X</div>
                    
                </div>

        


    </div>
 
  
</template>

<script>


export default {
    name:'MaModale',
    props:['revele', 'toggleModale'],
    
}
</script>

<style scoped  >

.bloc-modale{
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    width: 100%;    
    display: flex;
    justify-content: center;
    align-items: center;
}

.overlay{
    background: rgba(0,0,0,0.5);
    position: fixed;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
}

.modale{
    background: #ceb4b400;
    color: #333;
    padding: 40px;
    position: fixed;
    bottom: 10%;
    
}

.btn-modale {
    position: absolute;
    top: 10px;
    right: 10px;
}

#video-container{
    width: 800px;
    height: 380px;
}

@media (max-width: 780px ){
    #video-container{
    width: 500px;
    height: 320px;
}
.btn-modale {
    position: absolute;
    top: 10px;
    right: 10px;
}
}

@media (max-width: 500px ){
    #video-container{
    width: 300px;
    height: 400px;
}

.btn-modale {
    position: absolute;
    top: 10px;
    right: 10px;
}

}
</style>