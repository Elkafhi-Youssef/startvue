<template>
  <div>
<h2>hi {{name}} : {{heroName}}</h2>
  </div>
</template>

<script>
  export default {
    name:'Greet-Com',
    props:['name','heroName']
  }
</script>

<style scoped>

</style>
