<template>
  <div>
<h1> this is Popup</h1>
<button @click="$emit('close','youssef')">Close button</button>
  </div>
</template>

<script>
  export default {
    name:'Popup-P',
    emits:['close']
  }
</script>

<style scoped>

</style>