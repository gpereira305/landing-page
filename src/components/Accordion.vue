<template>
     <section class="accordion-component">
          <div class="accordion-wrapper"> 
              <h3>Dúvidas Frenquentes</h3>
             <ul uk-accordion="multiple: true">
                 <li class="uk-open">
                    <a class="uk-accordion-title" href="#"> 
                        <span>
                             Sou aluno CEISC dos cursos preparatório da 1 Fase do XXXII Exame e planos OAB. Preciso me increver? 
                        </span>  
                    </a>
                    <div class="uk-accordion-content">
                        <p> 
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus fugiat dignissimos provident, voluptate sint perferendis necessitatibus praesentium suscipit ipsum magnam culpa nisi id similique minima libero perspiciatis deleniti! Nemo ab dolorem reiciendis optio.
                        </p>
                    </div>
                </li>
                <li>
                    <a class="uk-accordion-title" href="#">
                         <span>
                             Sou aluno CEISC dos cursos preparatório da 1 Fase do XXXII Exame e planos OAB. Preciso me increver? 
                        </span>  
                    </a>
                    <div class="uk-accordion-content">
                        <p> 
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus fugiat dignissimos provident, voluptate sint perferendis necessitatibus praesentium suscipit ipsum magnam culpa nisi id similique minima libero perspiciatis deleniti 
                        </p>
                    </div>
                </li>
                <li>
                    <a class="uk-accordion-title" href="#">
                         <span>
                             Sou aluno CEISC dos cursos preparatório da 1 Fase do XXXII Exame e planos OAB. Preciso me increver? 
                        </span> 
                    </a>
                    <div class="uk-accordion-content">
                        <p> 
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus fugiat dignissimos provident, 
                        </p>
                    </div> 
                </li>
            </ul>
        </div>
     </section>
</template>



/* ============   JAVASCRIPT ==========  */
<script> 

export default {
  name: "Accordion", 
}
</script>



/* ============   STYLES  ==========  */
<style> 
 .accordion-component{ 
    background: var(--brand-blue-100);
    width: 100%;
    height: 65vh;
 }

 .accordion-component .accordion-wrapper{
     margin: 0 5%;
 }

 .accordion-wrapper{
    position: relative;
    top: 70px;
 }

 .accordion-wrapper h3{  
    color: var(--brand-blue);
    font-family: 'Quicksand', sans-serif;
    font-weight: 600;
    font-size: 2rem;
 }

 .accordion-wrapper li{ 
    border: 2px solid var(--brand-blue-800);
    border-radius: 10px; 
    padding: 5px 30px 17px;
 }

 .accordion-wrapper .uk-accordion-title { 
    font-size: 1.25rem;
    line-height: 1.4;
    color: var(--brand-black-600);
    overflow: hidden;  
    height: 55px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-flow: row-reverse;
}

 

.accordion-wrapper .uk-accordion-content{
    margin-top: 0;
}

.uk-accordion-title span,
.uk-accordion-content span{
   font-weight: 500;
}

.accordion-wrapper .uk-accordion-title::before{ 
    border: 2px solid var(--brand-blue-800);
    border-radius: 25px; 
} 

/*=========  1180px ============= */
@media screen and (max-width: 1180px){
    .uk-accordion-title::before{
        width: 31px;
        height: 28px;
    } 
    .accordion-wrapper .uk-accordion-title{
        font-size: 1.2rem;
    }
   .accordion-component {
        height: 70vh;
   }
}

/*=========  990px ============= */
@media screen and (max-width: 990px){
        .uk-accordion-title::before{
        width: 35px;
        height: 28px;
      } 
}

/*=========  820px ============= */
@media screen and (max-width: 820px){
        .uk-accordion-title::before{
        width: 24px;
        height: 20px; 
       } 
       .accordion-wrapper .uk-accordion-title {
           font-size: 1rem;
       }
       .uk-accordion-content>:last-child {
           font-size: .90rem;
       }
}


/*=========  690px ============= */
@media screen and (max-width: 690px){
    .accordion-wrapper h3 { 
        font-size: 1.5rem;
    }
     .uk-accordion-title::before { 
        height: 16px;
     }
     .accordion-component {
        height: 75vh;
    }
}

/*=========  520px ============= */
@media screen and (max-width: 520px){

    .accordion-wrapper li { 
        padding: 5px 14px 10px;
   }
   .uk-accordion-title::before {
        height: 14px;
   }
}

/*=========  420px ============= */
@media screen and (max-width: 420px){
  .accordion-wrapper .uk-accordion-title {
       height: 8vh;
       font-size: .85rem;
   } 
   .uk-accordion-title::before {
        height: 15px;
        width: 30px;
    }
    .accordion-component {
        height: 90vh;
    }
}

/*=========  320px ============= */
@media screen and (max-width: 320px){
    .accordion-component {
        height: 131vh;
   }
   .uk-accordion-title::before {  
        width: 41px;
   }
}

</style>