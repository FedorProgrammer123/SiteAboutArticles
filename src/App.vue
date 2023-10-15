<script setup>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Aside from './components/Aside.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <Header/>
  <Main/>
  <Aside/>
  <Footer/>
</template>
<script>
export default {
  components:{
    Header,
    Main,
    Aside,
    Footer
  }
}
</script>
<style>
*{
  margin: 0;
  padding: 0;
}
body{
  background-color: #F0EEF0;
}
</style>
