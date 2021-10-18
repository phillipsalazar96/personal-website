<template>
  <div class="about">
    <div class="flex flex-col  text-center">
      <div class="">
        <h2 class="font-title text-7xl mt-24">About</h2>
      </div>

      <div class="">
        <article class="font-par mt-6 md:w-1/3 m-auto px-12">
          Hello my name is Phillip Salazar, I am the web developer. I am a PHP developer that specialize in Laravel, VueJS, and WordPress.
          I worked on big and small projects and in several different industries too. 
        </article>
        
        <h4 class="font-title text-3xl mt-6" >Technologies</h4>
        <div class="md:w-96 m-auto" >
        <ul class="text-left ml-32">
          <li class="font-par">HTML, CSS, Javascript</li>
          <li class="font-par">PHP</li>
          <li class="font-par">MYSQL, SQL</li>
          <li class="font-par">Laravel</li>
          <li class="font-par">WordPress</li>
          <li class="font-par">VueJS</li>
          <li class="font-par">Jquery</li>
  
        </ul>
        </div>
      </div>

      <div class="">
        <p class="font-par mt-12 mb-12">Contact me at phillipsalazar96@gmail.com</p>
      </div>

    </div>
  </div>
</template>
<script>
// @ is an alias to /src


export default {
  name: 'About',
  components: {
    
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
