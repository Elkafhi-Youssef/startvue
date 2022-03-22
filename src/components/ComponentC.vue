<template>
  <div>
   <!-- <h2 :id=title >I'm in acticle: {{title}}</h2> -->
   <h2 >hi I'm a ComponentC</h2>
   <ComponentE/>
  </div>
</template>

<script>
import ComponentE from './ComponentE.vue'
  export default {
    name:'ComponentC-C',
    components:{
      ComponentE}
 
  }
</script>
