<template>
  <div class="about">
    <div class="flex flex-col  text-center">
        <div v-if="post" class="">
            <div class="">
                <h2 class="font-par text-7xl mt-24">{{post[0].title.rendered}}</h2>
            </div>

            <div class="mb-12">
                <article v-html="post[0].content.rendered" class="font-par mt-6 md:w-1/3 m-auto px-12">
                    
                </article>
                
            </div>
        </div>

        <div v-else class="mt-12">
            <p class="font-par text-3xl">No post...</p>
            <div class="mt-12 mb-12">
                <i class="fas fa-sad-cry fa-5x"></i>
            </div>
        </div>
    </div>
  </div>
</template>
<script>
// @ is an alias to /src
import axios from "axios";

export default {
  name: 'Post',
  components: {
    
  },
  data()
  {
      return {
          post: ''
      }
  },
  mounted()
  {
    axios.get("http://wordpress.test/wp-json/wp/v2/posts?slug=" + this.$route.params.slug).then((result) => {
      console.log(result.data);
     this.post = result.data;
    });
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
