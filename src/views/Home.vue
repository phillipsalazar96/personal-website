<template>
  <div class="home">
    <div class="homeheader">
      <div class="text-center font">
          <h1 class="text-7xl pt-80">Building Unique Digital experiences</h1>
          <p class="font2 mt-8 text-2xl" >The Web Developer</p>
        </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  components: {
    
  }
}
</script>
<style scoped>
  .homeheader
  {
    background: url('../assets/spash.jpg');
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-position: center;
    background-size: 2092px;
    box-shadow:inset 0 0 0 2000px hsla(266, 91%, 57%, 0.479);
    height: 826px;
    
  }

  .font
  {
    font-family: 'Mr Dafoe', cursive;
    color: white;
  }

  .font2
  {
    font-family: 'Yantramanav', sans-serif;
    color: white;
  }
</style>
