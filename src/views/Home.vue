<template>
  <div class="h-screen w-screen bg-primary flex flex-col">
      <NavBar></NavBar>
      <Advert></Advert>
      <Footer></Footer>
  </div>
</template>

<script>
import NavBar from '../components/NavBar.vue';
import Advert from '../components/Advert.vue';
import Footer from '../components/Footer.vue';
export default {
components:{
    NavBar,
    Advert,
    Footer
}
}
</script>

<style>

</style>