<template>
<div class="flex flex-col h-screen justify-between">
  <Header />
  <main class="body flex-grow">
    <router-view/>
  </main>
  <Footer />
  </div>
</template>
<script>

import Header from './components/Header';
import Footer from './components/Footer';

export default {
  components: {
    Header,
    Footer,

  },
  setup() {
    
  },
}
</script>

<style>


</style>
