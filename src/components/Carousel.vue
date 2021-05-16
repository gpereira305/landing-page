<template> 
  <section class="carousel-component">
      <div>
          <h3>Curso mentorado pelos professores</h3>
            <div class="uk-position-relative uk-visible-toggle uk-light carousel-slide" tabindex="-1" uk-slider>
              <ul class="uk-slider-items uk-child-width-1-2 uk-child-width-1-3@s uk-child-width-1-4@m">
                  <li>
                      <img class="carrousel-img" src="../assets/person.png" alt="person image"> 
                      <span class="teacher-name">Nidal Ahmad</span>
                  </li>
                  <li>
                      <img class="carrousel-img" src="../assets/person2.png" alt="person image"> 
                      <span class="teacher-name">Leonardo Fetter</span>
                  </li>
                  <li>
                      <img class="carrousel-img" src="../assets/person3.png" alt="person image"> 
                      <span class="teacher-name">Tatiana Marcello</span>
                  </li>
                  <li>
                      <img class="carrousel-img" src="../assets/person4.png" alt="person image"> 
                      <span class="teacher-name">Mateus Silveira</span>
                  </li>
                  <li>
                      <img class="carrousel-img" src="../assets/person5.png" alt="person image"> 
                      <span class="teacher-name">Andressa Antoninni</span>
                  </li>
                  <li>
                      <img class="carrousel-img" src="../assets/person6.png" alt="person image"> 
                      <span class="teacher-name">Paulo Lopes</span>
                  </li>
                  <li>
                      <img class="carrousel-img" src="../assets/person7.png" alt="person image">
                      <span class="teacher-name">Rodrigo Bastos</span>
                  </li> 
              </ul>
              <span class="elipse-icon left"></span>
              <span class="elipse-icon right"></span> 
              <a class="uk-position-center-left uk-position-small prev" href="#" uk-slidenav-previous uk-slider-item="previous"></a>
              <a class="uk-position-center-right uk-position-small next" href="#" uk-slidenav-next uk-slider-item="next"></a>
          </div>
     </div>
</section>
</template>

<script> 

export default {
    name: "Carousel", 
}


</script>

<style>

 .carousel-component{
    display: flex;
    flex-direction: column; 
    margin-bottom: 5%; 
 }

 .carousel-component:first-child div{
     margin-top: 20%;
 }

.carousel-component h3{
    margin: 47px 5%;
    color: #004FFF;
    font-family: 'Quicksand', sans-serif;
    font-weight: 600;
    font-size: 2rem;
}

 .carousel-component .carousel-slide{
       margin: 20px 5%!important;
 }

 .carousel-component li{
    display: flex;
    flex-direction: column;
    height: 89%;
    align-items: center;
    text-align: center; 
 }

 .carousel-component .carrousel-img{
    height: 270px;
    width: 100%;
    max-width: 270px;
 }

 .carousel-component .teacher-name{
    background: blue;
    padding: 15px;
    width: 51%; 
    border-top-right-radius: 25px;
    border-bottom-right-radius: 25px;
    border-top-left-radius: 25px;
    margin-top: -19px;
    z-index: 1;
    font-weight: 400;
    color: #fff;
    font-size: 1.2rem;
 } 

 .carousel-component .prev,
 .carousel-component .next{ 
    border-radius: 50%;
    padding: 14px;
    width: 20px;
    height: 20px;
    border: 2px solid #004FFF;
        top: 134.5px;
 }

 .carousel-component .elipse-icon{
    position: absolute; 
    border: 1px solid #004FFF; 
    transform: rotate(180deg);
    display: block;    
    width: 50px;
    background: #004FFF;
 }
 .carousel-component .elipse-icon.left{
    top: 136.2px;
    left: 39px;
 }
 .carousel-component .elipse-icon.right{ 
    right: 35px;
    bottom: 240.5px;
 }

 /* .carousel-component .arrow{
   position: absolute;
   left: 100%;
   right: -75%;
   top: 50%;
   bottom: 50%;
   border: 3px solid #004FFF;
   box-sizing: border-box;
   transform: rotate(180deg);
   display: block;
 } */

 svg:not(:root){
   position: absolute;
    left: 19px;
 }

 .uk-icon:not(.uk-preserve) [stroke*='#']:not(.uk-preserve){
   stroke: #004FFF;
 } 
</style>