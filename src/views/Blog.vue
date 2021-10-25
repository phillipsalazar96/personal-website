<template>
  <div class="blog">
    <div class="flex flex-col  text-center">
    


      <div v-for="post in posts" :key="post.id" class="">
            <div class="m-auto w-1/3">
                <a :href="'post/' + post.slug"><h2 class="font-par text-7xl mt-24">{{post.title.rendered}}</h2></a>
            </div>
            <article v-html="post.excerpt.rendered" class="font-par mt-6 md:w-1/3 m-auto px-12">
                
            </article>
  
      </div>

    </div>
  </div>
</template>
<script>
// @ is an alias to /src
import axios from "axios";

export default {
  name: 'Blog',
  components: {
    
  },
  data()
  {
      return {
          posts: ''
      }
  },
  mounted ()
  {
    
    axios.get("http://wordpress.phillipsalazar.com/wp-json/wp/v2/posts").then((result) => {
      console.log(result.data);
     this.posts = result.data;
    })
  }
  
}
</script>
<style scoped>

  .font-title
  {
    font-family: 'Mr Dafoe', cursive;
    color: black;
  }

  .font-par
  {
    font-family: 'Yantramanav', sans-serif;
    color: black;
  }
</style>
