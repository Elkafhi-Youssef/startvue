<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" url="you code "/> -->
  <!-- <h1> hi {{add()}}</h1> -->
  <!-- <h2 v-html="greate"></h2> -->
  <h1> {{fullname}}</h1>
  <h1> convert MAD USD</h1>
  <label >mad</label>
  <input type="number"   v-model="mad">
  <label >usd</label>
  <input type="number"   v-model="usd">
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
    return{
     first:'youssef',
     last:'elkafhi',
    mad:0,
    usd:0

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
    mad(v){
      this.usd = v/10;
    },
     usd(v){
      this.mad = v*10;
    }
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
