<script setup>
</script>

<template>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.0/css/all.min.css">


  <footer>
    <div class="container">
      <div class="row">
        <div class="col" id="company">

          <p>
            Este projeto visa ajudar as pessoas e empresas para terem melhor controle do estado <br>
            de conservação ideal
            para suas plantas,
          </p>
          <div class="social">
            <a href="#"><i class="fab fa-facebook"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-youtube"></i></a>
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-linkedin"></i></a>
            <a href="#"><i class="fab fa-local"></i></a>
          </div>
        </div>


        <div class="col" id="services">
          <h3>Páginas</h3>
          <div class="links">
            <a href="#">Sobre Nós</a>
            <a href="#">Equipe</a>
            <a href="#">Graficos</a>
            <a href="#">Graficos de Equipe</a>
          </div>
        </div>

        <div class="col" id="useful-links">
          <h3>Horários</h3>
          <div class="links">
            <a href="#">Segunda à Sexta ⬇</a>
            <a href="#">Horários: 7h às 18h</a>
            <a href="#">Sábados: 9h às 13h</a>
            <a href="#">Domingo: Fechado</a>
          </div>
        </div>

        <div class="col" id="contact">
          <h3>Contato</h3>
          <div class="contact-details">
            <i class="fa fa-location"></i>
            <p>BR-280 - Colégio Agrícola, 89245-000 <br> Santa Catarina, Araquari</p>
          </div>
          <div class="contact-details">
            <i class="fa fa-phone"></i>
            <p>+55 (47) 98804-2804</p>
          </div>
        </div>
      </div>

    </div>
  </footer>
</template>

<style scooped>
header {
  background-color: #000000;
  width: 100%;
  height: 5vh;
  padding: 1rem;
}

nav {
  display: flex;
  justify-content: space-between;
  color: black;
  width: 100%;
  height: 12vh;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;

}

footer {
  bottom: 0;
  background-color: #000000ff;
  position: absolute;
  width: 100%;
  min-height: 250px;
}

.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;


}

.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.col {
  margin-top: 5vh;
  min-width: 250px;
  color: #f2f2f2f2;
  font-family: poppins;
  padding: 0 2rem;
}

.col .logo {
  width: 100px;
  margin-bottom: 25px;
}

.col h3 {
  color: #ff014fff;
  margin-bottom: 20px;
  position: relative;
  cursor: pointer;
}

.col h3::after {
  content: '';
  height: 3px;
  width: 0px;
  background-color: #ff014fff;
  position: absolute;
  bottom: 0;
  left: 0;
  transition: 0.3s ease;

}

.col h3:hover::after {
  width: 30px
}

.col .social a i {
  color: #ff014fff;
  margin-top: 2rem;
  margin-right: 5px;
  transition: 0.3s ease;
}

.col .social a i:hover {
  transform: scale(1.5);
  filter: grayscale(25);
}

.col .links a {
  display: block;
  text-decoration: none;
  color: #f2f2f2;
  margin-bottom: 5px;
  position: relative;
  transition: 0.3s ease;
}

.col .links a::before {
  content: '';
  height: 16px;
  width: 3px;
  position: absolute;
  top: 5px;
  left: -10px;
  background-color: #ff014fff;
  transition: 0.5s ease;
  opacity: 0;
}

.col .links a:hover::before {
  opacity: 1;
}

.col .links a:hover {
  transform: translateX(-8px);
  color: #ff014fff;
}

.col .contact-details {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
}

.col .contact-details i {
  margin-right: 15px;
}

.row .form {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 2rem 0;
}

.row .form input {
  background-color: #1a1c20ff;
  border: 0;
  outline: none;
  padding: 14px 20px;
  border-radius: 6px;
  border-top-right-radius: 0;
  border-bottom-right-radius: 0;
}

.form button {
  padding: 14px 20px;
  border: 0;
  border-radius: 6px;
  border-top-left-radius: 0;
  border-bottom-left-radius: 0;
  background-color: #ff014fff;
}

/* Responsive Design */
@media(max-width:900px) {
  .row {
    flex-direction: column;
  }

  .col {
    width: 100%;
    text-align: left;
    margin-bottom: 25px;
  }
}

@media(max-width:768px) {
  .row {
    flex-direction: column;
  }

  .col {
    width: 100%;
    text-align: left;
    margin-bottom: 20px;
  }
}
</style>