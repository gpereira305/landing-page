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
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus fugiat dignissimos provident, voluptate sint perferendis necessitatibus praesentium suscipit ipsum magnam culpa nisi id similique minima libero perspiciatis deleniti! Nemo ab dolorem reiciendis optio magni incidunt nostrum nulla necessitatibus vero nihil, voluptate, corrupti veritatis ipsa temporibus sint quod minima nam sapiente dignissimos totam modi dolorum quisquam. Laudantium, mollitia. Ea, eos repudiandae?
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
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus fugiat dignissimos provident, voluptate sint perferendis necessitatibus praesentium suscipit ipsum magnam culpa nisi id similique minima libero perspiciatis deleniti! Nemo ab dolorem reiciendis optio magni incidunt nostrum nulla necessitatibus vero nihil, voluptate, corrupti veritatis ipsa temporibus sint quod minima nam sapiente dignissimos totam modi dolorum quisquam. Laudantium, mollitia. Ea, eos repudiandae?
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
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus fugiat dignissimos provident, voluptate sint perferendis necessitatibus praesentium suscipit ipsum magnam culpa nisi id similique minima libero perspiciatis deleniti! Nemo ab dolorem reiciendis optio magni incidunt nostrum nulla necessitatibus vero nihil, voluptate, corrupti veritatis ipsa temporibus sint quod minima nam sapiente dignissimos totam modi dolorum quisquam. Laudantium, mollitia. Ea, eos repudiandae?
                        </p>
                    </div> 
                </li>
            </ul>
        </div>
     </section>
</template>

<script>


export default {
  name: "Accordion"
}
</script>

<style>

 .accordion-component{ 
    background: #DFEFFF;
    width: 100%;
    height: 650px;
 }

 .accordion-component .accordion-wrapper{
     margin: 0 5%;
 }

 .accordion-wrapper{
    position: relative;
    top: 70px;
 }

 .accordion-wrapper h3{  
    color: #004FFF;
    font-family: 'Quicksand', sans-serif;
    font-weight: 600;
    font-size: 2rem;
 }

 .accordion-wrapper li{ 
    border: 2px solid blue;
    border-radius: 10px; 
    padding: 5px 30px 17px;
 }

 .accordion-wrapper .uk-accordion-title { 
    font-size: 1.25rem;
    line-height: 1.4;
    color: #333;
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
    border: 2px solid blue;
    border-radius: 25px; 
}

</style>