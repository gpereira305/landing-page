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

            <!-- BG -->
            <div class="info-form">
                <div class="info-text">
                  <h4>Se Prepare com o ceisc!</h4>
                  <h1>Aprenda como se preparar melhor para o Exame da OAB</h1>

                  <div class="detailed-info">

                    <div class="info-group">
                      <span>Início:</span>
                      <span>25/05/2021</span>
                    </div>
                    <div class="info-group">
                      <span>Valor:</span>
                      <span>Curso Gratuito</span>
                    </div>
                    <div class="info-group">
                      <span>Assista aonde:</span>
                      <span>Plataforma Ceisc</span>
                    </div>
                      <div class="info-group">
                        <div>
                            <span><i class="fas fa-chevron-right"></i></span>
                            <span><i class="fas fa-chevron-right"></i></span>
                            <span><i class="fas fa-chevron-right"></i></span>
                        </div>
                      </div>
                  </div>
                </div>
 
                  <form action="#">
                    <h3>Inscreva-se e fique por dentro!</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi eveniet, perspiciatis sunt fuga nemo quod soluta dignissimos aliquid nihil corporis?</p>
                    <input  name="name" ref="name"  type="text" placeholder="Nome Completo" required> 
                    <input  name="email" ref="email"  type="email" placeholder="E-mail" required>   
                    <button @click="handleSubmit"  type="button">
                      Quero!
                    </button>
                  </form> 
            </div> 
      </section>
</template>

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
  background: #fff;
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
    color: #00956A;
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

}

.info-form .info-text h4{
  color: #FFB100;
  text-transform: uppercase;
  font-size: 1.5rem;
}

.info-form .info-text h1{
    line-height: 1.3;
    color: #fff;
    font-size: 4.5rem;
    width: 83%;
}

.info-form form{
    display: flex;
    flex-direction: column;
    background: #fff;
    padding: 3.5rem;
    height: 550px;
    border-radius: 10px;
    box-shadow: 0px 3px 65px 3px rgb(0 0 111);
}

.info-form form h3{
    margin-top: 0;
    font-size: 2rem;
    text-align: center;
    margin-bottom: 0;
}

.info-form form p{
  margin-bottom: 5rem;
}

.info-form form input{ 
  height: 70px;
  outline: none;
  margin-bottom: 2rem;
  border: 1.8px solid #737380;
  border-radius: 5px;
  font-size: 1.2rem;
  padding: 0 10px;
  color: #737380;
}

.info-form form input:focus{
   border: 2px solid #004FFF;
}

.info-form form input::placeholder{
  color: #737380;
}

.info-form form input:last-of-type{
      margin-bottom: 3.5rem;
}

.info-form button{
  height: 70px;
  cursor: pointer;
  outline: none;
  border: none;
  color: #fff;
  background: #00956A;
  font-size: 1.2rem;
  text-transform: uppercase;
  transition: all ease .4s;

}

.info-form button:hover{
  background: #017a58;
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

.info-group span{
  color: #fff;
}

.info-group .fas{
  font-size: 2.5rem;
  color: #6699cc;
}

</style>