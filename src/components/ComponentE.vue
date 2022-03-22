<template>
  <div>
   <!-- <h2 :id=title >I'm in acticle: {{title}}</h2> -->
   <h2 >hi I'm a ComponentE</h2>
   <ComponentF/>
  </div>
</template>

<script>
import ComponentF from './ComponentF.vue'
  export default {
    name:'ComponentE-E',
    components:{
      ComponentF
    }

 
  }
</script>