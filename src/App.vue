<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <a class="navbar-brand" href="#">MiPortafolio</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <!-- Usamos Flexbox para alinear los enlaces a la derecha en pantallas grandes y centrar en pequeñas -->
        <ul class="navbar-nav ml-auto w-100 justify-content-center justify-content-lg-end">
          <li class="nav-item active">
            <a class="nav-link" href="#home">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#about">About me</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#gallery">Gallery</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#contact">Contact</a>
          </li>
        </ul>
      </div>
    </nav>

    <HomePage />
    <AboutMe />
    <ProjectGallery />
    <ContactForm />
  </div>
</template>

<script>
// Importaciones de los componentes
import HomePage from './components/HomePage.vue';
import AboutMe from './components/AboutMe.vue';
import ProjectGallery from './components/ProjectGallery.vue';
import ContactForm from './components/ContactForm.vue';

export default {
  name: 'App',
  components: {
    HomePage,
    AboutMe,
    ProjectGallery,
    ContactForm
  }
}
</script>

<style>
/* Estilos globales */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0;
}

nav {
  margin-bottom: 20px;
}

/* Estilos adicionales para que sea responsivo */
.navbar-nav {
  display: flex;
  justify-content: flex-end;
  width: 100%;
  padding-left: 0;
}

@media (max-width: 767px) {
  .navbar-nav {
    justify-content: center; 
  }
}

/* Ajuste general para el contenedor de la página */
#app {
  padding: 0 15px;
}

@media (max-width: 991px) {
  #app {
    padding-left: 10px;
    padding-right: 10px;
  }
}
</style>
