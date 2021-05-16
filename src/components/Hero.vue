<template>
      <section class="main-section">
           <div class="overlay"></div>
           <div class="overlay-confirmation">
             <!-- Modal -->
             <div class="modal">
                <div>
                  <h2>Uhu!</h2>
                  <h2>Cadastro foi feito com sucesso</h2>
                </div>
                 <div class="check-sign">
                   <i class="far fa-check-circle"></i>
                 </div>

                 <div>
                   <p>Confira seu e-mail para mais detalhes</p>
                 </div>
             </div>
           </div>
              <!-- Header -->
            <header>
              <img src="../assets//logo_wht.png" alt="logo">
            </header>

            <!-- Main background -->
            <div class="info-form">
                <div class="info-text" data-aos="fade-right">
                  <h4>Se Prepare com o ceisc!</h4>
                  <h1>Aprenda como se preparar melhor para o Exame da OAB</h1>

                  <div class="detailed-info">
                    <div class="info-group">
                      <p>Início:</p>
                      <p>25/05/2021</p>
                    </div>
                    <div class="info-group">
                      <p>Valor:</p>
                      <p>Curso Gratuito</p>
                    </div>
                    <div class="info-group">
                      <p>Assista aonde:</p>
                      <p>Plataforma Ceisc</p>
                    </div>
                      <div class="info-group">
                        <div>
                            <span><i class="fas fa-chevron-right"></i></span>
                            <span><i class="fas fa-chevron-right middle"></i></span>
                            <span><i class="fas fa-chevron-right last"></i></span>
                        </div>
                      </div>
                  </div>
                </div>
                  <!-- Form  -->
                  <form action="#" data-aos="zoom-in-left" data-aos-duration="1500">
                    <h3>Inscreva-se e fique por dentro</h3>
                    <p>
                      Cadastre-se para receber conteúdos exclusivos sobre como se preparar melhor para esse grande dia. Não fique de fora.
                    </p>
                    <input  name="name" ref="name"  type="text" placeholder="Nome Completo" required> 
                    <input  name="email" ref="email"  type="email" placeholder="E-mail" required>   
                    <button @click="handleSubmit"  type="button">
                      Quero!
                    </button>
                  </form> 
            </div> 
      </section>
</template>

/* ============   JAVASCRIPT ==========  */
<script> 

export default {
  name: "Hero", 

  data(){
       return {
       name: "",
       email: ""
      }
  },

  methods: {  
      handleSubmit(){  
        if(this.$refs.name.value === ""){
          alert("Nome é obrigatório")
        } else if(this.$refs.email.value === ""){
          alert("E-mail é obrigatório") 

        }else{
          // On submit, shows a successful message for 3 seconds 
          const showMsg = document.querySelector(".overlay-confirmation");  
          showMsg.style.display = "flex";  
           setTimeout(() => { 
           showMsg.style.display = "none";
           this.$refs.name.value = "" ;
           this.$refs.email.value = "" ;
         }, 3000) 
          
        }
          
     }
  }
}
</script>


/* ============   STYLES ==========  */
<style>


.overlay{
  position: absolute;
  top: 0;
  bottom: 0;
  height: 100vh;
  width: 100%;
  background: rgb(0 79 255 / 80%);
   transition: all ease-in-out .7s;
}

.overlay-confirmation{
  position: fixed;
  top: 0;
  bottom: 0;
  height: 100vh;
  width: 100%;
  background: rgb(0 0 0 / 80%);
  z-index: 100;
  display: flex; 
  justify-content: center;
  align-items: center;
  display: none; 
 
}

.overlay-confirmation .modal{
  background: var(--brand-black-100);
  width: 500px;
  height: 400px;
  border-radius: 5px;
  padding: 30px;
  font-family: 'Quicksand', sans-serif; 
}

.modal:first-child div{
  margin-bottom: 6.5rem;
}

.modal h2{
  font-weight: 600;
}

.modal p{
    font-weight: 600;
    font-size: 1.2rem;
    text-align: center;
}

.modal h2:last-child{
  margin: 0;
}

.modal .check-sign{
    display: flex;
    justify-content: center;
    font-size: 5rem;
    color: var(--brand-success);
    margin-bottom: 10rem;

}

.main-section{
  background-image: url("../assets/main_bg.png");
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}

.main-section  header{
  padding: 30px 5%;
 } 

.main-section img{
    position: relative;
    max-width: 270px;
    width: 100%;
    height: 70px;
} 

.info-form{ 
  position: relative;
  display: flex; 
  width: 90%;
  margin: auto; 
  height: 83vh;
}

.info-form .info-text{
  width: 100%;
  margin-top: 70px;

}

.info-form .info-text h4{
  color: var(--brand-warning);
  text-transform: uppercase;
  font-size: 1.5rem;
  font-weight: 500;
}

.info-form .info-text h1{
    line-height: 1.3;
    color: var(--brand-black-100);
    font-size: 4.5rem;
    width: 83%;
    font-family: 'Lexend', sans-serif; 
    font-weight: 800;
}

.info-form form{
    display: flex;
    flex-direction: column;
    background: var(--brand-black-100);
    padding: 3.5rem;
    height: 550px;
    border-radius: 10px;
    box-shadow: 0px 3px 65px 3px rgb(0 0 111);
}

.info-form form h3{
    margin-top: 0;
    font-size: 2rem;
    text-align: left;
    margin-bottom: 0;
    font-weight: 600;
    font-family: 'Quicksand', sans-serif; 
}

.info-form form p{
    margin-bottom: 4rem;
    font-size: 1.1rem;
    font-weight: 600;
    font-family: 'Quicksand', sans-serif; 
}

.info-form form input{ 
  height: 70px;
  outline: none;
  margin-bottom: 2rem;
  border: 1.9px solid var(--brand-black-300);
  border-radius: 5px;
  font-size: 1.2rem;
  padding: 0 30px;
  color: var(--brand-black-600);
}

.info-form form input:focus{
   border: 2px solid var(--brand-blue);
}

.info-form form input::placeholder{
  color: var(--brand-black);

}

.info-form form input:last-of-type{
      margin-bottom: 3.5rem;
}

.info-form button{
  height: 70px;
  cursor: pointer;
  outline: none;
  border: none;
  color: var(--brand-black-100);
  background: var(--brand-success);
  font-size: 1.2rem;
  text-transform: uppercase;
  transition: all ease .4s;

}

.info-form button:hover{
  background: var(--brand-success);
}

.detailed-info{
    display: grid;
    grid-template-columns:  25% 25% 36% 13%;
}

.detailed-info .info-group{ 
    grid-template-rows: 10%; 
    display: flex;
    flex-direction: column;
}

.info-group p{
  color: var(--brand-black-100);
  margin: 0;
  font-size: 1.2rem;
}

.info-group p:nth-of-type(2){
  font-weight: 500;
}

.info-group .fas{
  font-size: 2.5rem;
  color: #6c96f5;
}

.info-group .fas.middle{
  color: rgb(191 208 243 / 97%);
}
.info-group .fas.last{
  color: var(--brand-black-100);
}

/*=========  1450px ============= */
@media screen and (max-width: 1450px) { 
    .info-form .info-text h1{
      font-size: 3.5rem;
    }
    .info-form form {
      height: 480px;
      width: 670px;
    }
    .info-form form h3 {
      font-size: 1.7rem;
    }

    .info-form form p{
      margin-bottom: 2rem;
    }

    .detailed-info {
      grid-template-columns: 20% 20% 30% 15%;
    }
    .info-group p { 
        font-size: 1rem;
    }
    .info-group .fas{
      font-size: 2rem;
    }

}

/*=========  1180px ============= */
@media screen and (max-width: 1180px){
  .info-form .info-text h4 {  
    font-size: 1.2rem; 
  }
    .info-form form {
      height: 450px;
      margin-top: 7%;
    }

    .info-form .info-text h1 {
      font-size: 3rem;
    }
    .detailed-info { 
    display: flex;
    flex-direction: column;
    }
 
   .detailed-info .info-group { 
    padding-bottom: 13px; 
   }
} 

/*=========  990px ============= */
@media screen and (max-width: 990px){
    .main-section img { 
      max-width: 200px; 
      height: 48px;
    }
    .info-form { 
      display: flex;
      flex-direction: column; 
      height: 130vh;
      margin-bottom: 10%;
    }
    .info-form form{
      width: 500px;
      margin: auto;
    }
    .info-form .info-text { 
      margin-bottom: 10%;
    }
   .detailed-info{
      display: flex;
      flex-direction: row;
      justify-content: space-between  ;
   }
    .main-section{
      background-image: none;
      height: auto;
    }
    .overlay { 
      height: 155vh;
    } 
}

/*=========  690px ============= */
@media screen and (max-width: 690px){
  .info-form form {
      width: 80%;
      height: 400px;
      padding: 2rem;
   }
   .info-form form h3 {
      font-size: 1.5rem;
   }
   .info-form form p {
      margin-bottom: 1rem;
      font-size: 1rem;
  }
  .info-form form input:last-of-type {
      margin-bottom: 20px;
  }
  .detailed-info {
      grid-template-columns: 25% 25% 36% 13%;
  }
  .overlay-confirmation .modal{
    width: 70%;
    height: 350px;
  }
  .modal .check-sign {
    margin-bottom: 7rem;
  }
  .modal:first-child div { 
       margin-bottom: 4rem;
  }
}

/*========= 520px ============= */
@media screen and (max-width: 520px){
  .main-section img {
    max-width: 180px; 
  }
  .info-form .info-text h1 { 
    font-size: 3rem;
    width: 100%; 
  }
  .info-form form input,
  .info-form button {
    font-size: 1rem;
  } 
  .info-group p {
    font-size: .8rem;
  }
  .info-group .fas {
   font-size: 1.5rem;
  }
  .modal .check-sign {
    font-size: 4.5rem;
  }
   .modal h2 {
     font-size: 1.5rem;
   }
   .modal p {
     font-size: 1rem;
   }
}

/*========= 420px ============= */
@media screen and (max-width: 420px){
  .overlay { 
    height: 173vh;
  } 
  .overlay-confirmation .modal {
    width: 76%;
    height: 300px;
  }
  .info-form{ 
     height: 149vh;
  }
   
  .info-form form { 
    margin: 10px auto;
  }
  .info-form .info-text h1 {
    font-size: 2.5rem; 
  } 
  .detailed-info .info-group:last-child { 
    display: none;
  }
  .modal:first-child div {
    margin-bottom: 3rem;
  }
  .modal h2 {
    font-size: 1.3rem;
  }
  .modal .check-sign {
    font-size: 4rem;
  }

}

/*========= 320px ============= */
@media screen and (max-width: 320px) {
    .overlay { 
       height: 205vh;
    }   
    .info-form {
      height: 178vh;
    }

}


</style>