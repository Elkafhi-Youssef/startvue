<template>
  <div>
   <TemplateRef/>
  </div>
</template>

<script>
import TemplateRef from "./components/TemplateRef.vue";
// import CreatePost from "./components/CreatePost.vue";

export default {
  name: "App",
  components:{TemplateRef},
  data() {
    return {
      name:'',
    };
  },
  methods: {
  },
  computed: {
  },
  watch: {
  },
  provide:{
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
