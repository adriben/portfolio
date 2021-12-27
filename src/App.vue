<template>
 <Spinner v-if="isLoading"></Spinner>
    <router-view/>
     
  
</template>

<script>
import Spinner from '@/components/Spinner.vue';


export default {
 name: 'app',
 data(){
    return {
      isLoading: true
    }
 },
 components: {
   "Spinner": Spinner
 },
  mounted () {
      this.$nextTick(() => {
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
