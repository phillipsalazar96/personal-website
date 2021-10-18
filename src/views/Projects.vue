<template>
  <div class="projects">
      <div class="flex flex-col text-center">
          <div class="">
              <h2 class="font-title text-7xl mt-24">Projects</h2>
            </div>
            <div class="">
                <p class="font-par mt-12">No projects currently...</p>
                <div class="mt-12">
                    <i class="fas fa-sad-cry fa-5x"></i>
                </div>
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