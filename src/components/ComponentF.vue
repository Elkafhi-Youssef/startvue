<template>
  <div>
   <!-- <h2 :id=title >I'm in acticle: {{title}}</h2> -->
   <h2 >hi I'm a ComponentF</h2>
   <h3 >F username : {{username}}</h3>
  </div>
</template>

<script>
  export default {
    name:'ComponentF-F',
    inject:['username']
  }
</script>