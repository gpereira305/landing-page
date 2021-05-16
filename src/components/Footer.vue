<template>
  <section class="footer">
        <footer>
            <span>
                <img src="../assets//logo.png" alt="logo">
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

<script>
export default {
    name: "Footer",

}
</script>

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
  width: 35%;
  justify-content: space-between;
  align-items: center;
} 

.footer .social-media h4{ 
    margin-bottom: 0;
    color: #004FFF;
    font-weight: 500;
}

.social-media .media-links a{
    text-decoration: none;
    font-size: 1.3rem;
    margin: 0 15px;
    color: #404040;
} 


.social-media .media-links a:last-child{
    margin-right: 0;
}
</style>