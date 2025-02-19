<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark px-3">
      <a class="navbar-brand" href="#">MiPortafolio</a>
      <div class="d-flex ms-auto">
        <ul class="navbar-nav">
          <li class="nav-item">
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

    <section id="home">
      <HomePage />
    </section>
    <section id="about">
      <AboutMe />
    </section>
    <section id="gallery">
      <ProjectGallery />
    </section>
    <section id="contact">
      <ContactForm />
    </section>
  </div>
</template>

<script>
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

.navbar-nav {
  display: flex;
  justify-content: flex-end;
}

.navbar-nav .nav-link {
  color: white;
  font-size: 16px;
  padding: 10px;
}

/* Reducir padding*/
section {
  padding: 30px 0; /* Espacio entre el encabezado y mi informacion */
}

</style>
