<template>
  <div>
   <!-- <Article title="myarticle"/> -->
    <!-- <Greet :name="first" heroName="batman" />
    <Greet name="abdo" heroName="batman1"/>
    <Greet name="zaynab" heroName="batman2" /> -->
    <!-- <ComponentC /> -->
    <button @click="showPopup = true">Show Popup</button>
    <Popup v-show="showPopup" @close="closePopup"/>
    
    
  </div>
</template>

<script>
import Popup from "./components/Popup.vue";
// import ComponentC from "./components/ComponentC.vue";

export default {
  name: "App",
  components:{Popup},
  data() {
    return {
      showPopup:false
      
    };
  },
  methods: {
    closePopup(n){
      this.showPopup = false
     console.log('name',n);
    }
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
