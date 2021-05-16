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





<script>
export default {
  name: "HeroBottom", 
}
</script>

<style>
.hero-bottom{
  position: absolute; 
  width: 100%;
  background: #004FFF;
  margin: auto;
  /* margin-top: 8rem; */

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
    color: #fff;
}


</style>