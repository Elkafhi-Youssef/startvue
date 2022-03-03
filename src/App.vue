<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" url="you code "/> -->
  <!-- <h1> hi {{add()}}</h1> -->
  <!-- <h2 v-html="greate"></h2> -->
  <h1> {{fullname}}</h1>
  <h1> convert MAD USD</h1>
  <label >Hour</label>
  <input type="number"   v-model="h">
  <label >minute</label>
  <input type="number"   v-model="m">
  <label >second</label>
  <input type="number"   v-model="s">
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
    return{
     first:'youssef',
     last:'elkafhi',
    h :0,
    m:0,
    s:0,

    }
  },
  methods:{
    add(){
      return 1+2;
    }
  },
  computed:{
    fullname(){
      return `${this.first}`
    }
  },
  watch:{
    h(v){
      this.m = v*60;
      this.s = v*60*60;
    }, 
    m(v){
      this.h = v/60;
      this.s = v*60;
    },
     s(v){
      this.m = v/60;
      this.h = v/3600;
    },
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
