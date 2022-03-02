<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" url="you code "/> -->
  <!-- <h1> hi {{add()}}</h1> -->
  <!-- <h2 v-html="greate"></h2> -->
  <h1> {{fullname}}</h1>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
    return{
     first:'youssef',
     last:'elkafhi'
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
