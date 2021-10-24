<template>
  <div class="">
      <header class="headerbar">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4 ">
            <div class="">
                <h1 class="header-text text-5xl  md:ml-36" >Phillip Salazar</h1>
            </div>
            
            <div id="nav" class="md:justify-self-end flex flex-col text-2xl mt-2 mr-12 sm:text-center md:flex-row">
                <router-link to="/" class="links md:mx-6">Home</router-link> |
                <router-link to="/projects" class="links md:mx-6" >Projects</router-link> |
              <!--  <router-link to="/blog" class="links md:mx-6" >Blog</router-link> | -->
                <router-link to="/about" class="links md:mx-6" >About</router-link>
            </div>
        </div>
    </header>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>




.header-text
{
    font-family: 'Mr Dafoe', cursive;
}

.links 
{
    font-family: 'Yantramanav', sans-serif;
  
}

.headerbar
{
    background: rgba(124, 58, 237);
    color: white;
    padding: 30px;
}
</style>
