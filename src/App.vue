<template>
<div v-if="isLoading" class="loader">
  <CubeShadow class="spin"></CubeShadow>
    </div>
    
     <router-view/>
   
     
  
</template>

<script>
import {CubeShadow} from 'vue-loading-spinner';


export default {
 name: 'app',
 data(){
    return {
      isLoading: true
    }
 },
 components: {
 "CubeShadow": CubeShadow
 },
 mounted () {
         
         window.addEventListener("load", async () => {    
       this.isLoading = false
})
      
    }

    
  
}
</script>


<style lang="scss">
*{
  margin: auto;
  max-width: 1900px;
}


.btn{
  border-radius: 20px;
}

.btn-primary{
  background-color: rgb(44, 117, 81);
  &:hover{
background-color: rgb(77, 158, 117);
color: black;
  }
}


</style>
