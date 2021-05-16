<template>
  <section class="footer">
        <footer>
            <span>
                <img src="../assets/logo.png" alt="logo">
            </span>

            <div class="social-media"> 
            <h4>Siga o Ceisc nas Redes Sociais</h4>
            <div class="media-links">
                <a href="http://www.facebook.com" target="_blank" rel="noopener noreferrer">
                  <i class="fab fa-facebook-f"></i> 
                </a>
                <a href="http://www.twitter.com" target="_blank" rel="noopener noreferrer">
                  <i class="fab fa-twitter"></i> 
                </a>
                <a href="http://www.instagram.com" target="_blank" rel="noopener noreferrer">
                  <i class="fab fa-instagram"></i> 
                </a>
                <a href="http://www.youtube.com" target="_blank" rel="noopener noreferrer">
                  <i class="fab fa-youtube"></i> 
                </a>
                <a href="http://www.linkedin.com" target="_blank" rel="noopener noreferrer">
                  <i class="fab fa-linkedin-in"></i> 
                </a> 
            </div>
            </div>
        </footer>
  </section>
</template>


/* ============   JAVASCRIPT ==========  */
<script>
export default {
    name: "Footer",

}
</script>


/* ============   STYLES ==========  */
<style>

.footer{
  margin: 0 5%;
}

.footer footer{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 0;
}

.footer img{
   max-width: 150px;
   width: 100%;
}

.footer .social-media{
  display: flex; 
  justify-content: space-between;
  align-items: center;
} 

.footer .social-media h4{ 
    margin-bottom: 0;
    color: var(--brand-blue);
    font-weight: 500;
}

.social-media .media-links a{
    text-decoration: none;
    font-size: 1.3rem;
    margin: 0 15px;
    color: var(--brand-black-600);
} 


.social-media .media-links a:last-child{
    margin-right: 0;
}

/*=========   990px ============= */
@media screen and (max-width:  990px){
    .footer img {
      max-width: 120px; 
   }
   .footer .social-media h4{
     font-size: 1rem;
   }
   .social-media .media-links a { 
      font-size: 1rem;
      margin: 0 12px; 
   }
}

 
/*=========  690px ============= */
@media screen and (max-width: 690px){
  .footer .social-media {  
      flex-direction: column;
  }

}

/*=========  420px ============= */
@media screen and (max-width: 420px){
  .footer footer {  
    align-items: center;
    padding: 20px;
    flex-direction: column;
   }

.footer img {
    max-width: 110px;
    margin-bottom: 15px;
  }
}
 

</style>