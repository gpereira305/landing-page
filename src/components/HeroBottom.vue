<template>
     <section class="hero-bottom">
         <article class="bottom-text">
            <div class="text-group">
                <p style="padding-bottom: 1rem">
                  O curso de preparação para o Exame de Ordem é totalmente focado
                  em estudantes que já são estão se preparando para prestar o Exame. 
                </p> 
                <p>
                  Você vai aprender técnicas para memorizar o principal conteúdo, técnicas
                  de como manter a calma nesse momennto e "hacks" incríveis que te darão um impulso no dia do exame!
               </p>
            </div>

            <div class="text-group2">
                <p>
                 Ao se inscrever no curso e se preparar, você ainda pode ganhar bolsas de estudo para cursos
                 Ceisc, durante as transmissão das lives durante a semana.
                 </p>
            </div>
      </article>
     </section>
</template>


/* ============  JAVASCRIPT ==========  */
<script> 

export default {
  name: "HeroBottom",  
  
}
</script>


/* ============   STYLES  ==========  */
<style> 

.hero-bottom{ 
  width: 100%;
  background: var(--brand-blue);
  margin: auto; 
  height: 45vh;

}

.bottom-text{
  width: 90%;
  margin: auto;
  display: grid; 
  grid-template-columns: 43% 32% auto;
  grid-gap: 25%;
  padding: 5% 0;
}

.bottom-text .text-group{
    padding-right: 15%;
}
.bottom-text .text-group2{
    padding-left: 27%;
}

.bottom-text p{
    color: var(--brand-black-100);
}


/*=========  990px ============= */
@media screen and (max-width: 990px){
    .bottom-text {
      display: flex;
      grid-gap: 0;
    } 
    .bottom-text .text-group2 {
      padding-left: 0;
   }
}


/*========= 520px ============= */
@media screen and (max-width: 520px){
   .bottom-text { 
    flex-direction: column;
  }
  .bottom-text p{
      font-size: .9rem;
   }
  .bottom-text .text-group{
    padding-right: 0;
  }
}


/*========= 420px ============= */
@media screen and (max-width: 420px){
   .hero-bottom{
     height: 45vh;
   }
}

/*========= 320px ============= */
@media screen and (max-width: 320px){
  .hero-bottom { 
       height: 60vh;
  }
}


</style>