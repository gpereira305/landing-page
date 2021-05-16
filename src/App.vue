<template>
   <div id="app">
     <div class="container hero"><Hero/></div> 
       <div class="container"><HeroBottom/></div>
       <div class="container"><Carousel/> </div>
       <div class="container"><Accordion/></div>
       <div class="container"><Footer/></div> 
  </div>
</template>


/* ============   JAVASCRIPT ==========  */
<script>  
import Hero from "./components/Hero";
import HeroBottom from "./components/HeroBottom";
import Carousel from "./components/Carousel"; 
import Accordion from "./components/Accordion";
import Footer from "./components/Footer";

import AOS from 'aos';
import 'aos/dist/aos.css';

export default {
  name: 'App',
  components: { 
    Hero, 
    HeroBottom,
    Carousel, 
    Accordion,
    Footer
  }, 
  data(){
    return{},
       AOS.init({
     once: true,
     easing: 'ease',
     delay: 300,
     duration: 2000,
   });
  }
}


</script>

/* ============  STYLES  ==========  */
<style>

/* =========== COLOR VARIABLES =========== */
 :root{
   --brand-blue-800: #00309D;
   --brand-blue: #004FFF;
   --brand-blue-100: #DFEFFF;
   --brand-black: #0C0C0C; 
   --brand-black-600: #404040;
   --brand-black-300: #C8C9CD;
   --brand-black-100: #F6F9FC;
   --brand-danger: #FF6B5F;
   --brand-danger-400: #FF9C8F;
   --brand-danger-100: #FFE0DC;
   --brand-warning: #FFB100;
   --brand-warning-400: #FFDA00;
   --brand-warning-100:#FFF7E5;
   --brand-success: #00956A;
   --brand-success-400: #00C592;
   --brand-success-100: #BCE0DB;
 }
/* ====================================== */

html, body{
  overflow-x: hidden;
  height: 100vh;
  width: 100vw;
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
