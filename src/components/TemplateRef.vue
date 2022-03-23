<template>
  <div>
  <input type="text" ref="inputRef" id="">
  </div>
</template>

<script>
  export default {
    name:'TemplateRef',
    mounted(){
      this.$refs.inputRef.focus()
    }
  }
</script>

<style scoped>

</style>