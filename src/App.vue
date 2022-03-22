<template>
  <div>
   <!-- <Article title="myarticle"/> -->
    <!-- <Greet :name="first" heroName="batman" />
    <Greet name="abdo" heroName="batman1"/>
    <Greet name="zaynab" heroName="batman2" /> -->
    <ComponentC />
    
    
  </div>
</template>

<script>
// import Greet from "./components/Greet.vue";
import ComponentC from "./components/ComponentC.vue";

export default {
  name: "App",
  components:{ComponentC},
  data() {
    return {
      first: "youssef",
      
    };
  },
  methods: {
    
  },
  computed: {
    
  },
  watch: {
    
  },
  provide:{
    username:'sajoselva'
  }
};
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
