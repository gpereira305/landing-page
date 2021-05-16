<template>
   <div id="app">
     <div class="container"><Hero/></div> 
       <div class="container"><HeroBottom/></div>
       <div class="container"><Carousel/> </div>
       <div class="container"><Accordion/> </div>
       <div class="container"><Footer/></div> 
  </div>
</template>

<script>  
import Hero from "./components/Hero";
import HeroBottom from "./components/HeroBottom";
import Carousel from "./components/Carousel"; 
import Accordion from "./components/Accordion";
import Footer from "./components/Footer";

export default {
  name: 'App',
  components: { 
    Hero, 
    HeroBottom,
    Carousel, 
    Accordion,
    Footer
  }
}
</script>




<style>
html, body{
  overflow-x: hidden;
  height: 100%;
  padding: 0;
  margin: 0;
  box-sizing: border-box; 
  scroll-behavior: smooth; 
} 

.container{
    width: 100%;
    height: 100%;
    position: relative;
}


</style>
