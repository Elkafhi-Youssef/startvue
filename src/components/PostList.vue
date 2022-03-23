<template>
  <div>
    
    <div v-for="post in posts" :key="post.id">
    <h3>{{post.id}}.{{post.title}}</h3>
    <p>{{post.body}}</p>
    <h3 v-if="errormessage">{{errormessage}}</h3>
    <hr/>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
  export default {
    name:'PostList-com ',
    data(){
      return{
        posts:[],
        errormessage:''
      }
    },
    created(){
      this.getPosts()
    },
    methods:{
      getPosts(){
        axios.get('https://jsonplaceholder.typicode.com/posts')
        .then(response =>{
          console.log(response.data);
          this.posts = response.data;
        })
        .catch(error=>{
          console.log(error);
          this.errormessage='Error retriving data'
        })
      }
    }
  }
</script>

<style scoped>

</style>
