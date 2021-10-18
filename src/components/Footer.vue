<template>
  <div class="footerbar">
      <footer class="footer-text">
        Developed by: <span class="footer-title">Phillip Salazar</span> | &copy; {{date}}
      </footer>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  setup()
  {
      return {
          date: new Date().getFullYear()
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.footer-title
{
    font-family: 'Mr Dafoe', cursive;
}

.footer-text
{
    font-family: 'Yantramanav', sans-serif;
    text-align: center;
    
}

.footerbar
{
    background: rgba(124, 58, 237);
    color: white;
    padding: 30px;
}
</style>
