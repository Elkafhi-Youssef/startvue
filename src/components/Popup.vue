<template>
  <div>
<h1> this is Popup</h1>
<input type="text" name="" v-model="name" id="">
<button @click="$emit('close',name)">Close button</button>
  </div>
</template>

<script>
  export default {
    name:'Popup-P',
    emits:{
      close:(name)=>{
        if(!name){
          return false 
        }else {
          return true
        }
    }
    },
    data(){
      return {
        name: '',
      }
    }
  }
</script>

<style scoped>

</style>