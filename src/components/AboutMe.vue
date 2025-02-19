<template>
  <div id="about" class="about-section">
    <div class="about-container">
      <!-- Imagen a la izquierda -->
      <div class="about-img-container">
        <img src="@/assets/fotoyo.jpg" alt="Foto" class="about-img" />
      </div>

      <!-- Información a la derecha -->
      <div class="about-info">
        <h2>Sobre mí</h2>
        <p>Mi nombre es Carlos Eduardo Martinez Hernandez, actualmente tengo 21 años me apasiona aprender cosas nuevas
          para poder superarme, tengo talento en aprender rápido las cosas y aplicarlas, también me gusta organizar equipos, soy estudiante universitario
          en la Universidad de la Riviera Maya de la carrera de Entornos virtuales, me agrada mucho el querer aprender a programar y diseñar al igual trabajo
          como Gerente en McDonalds con una carrera ya creada ahí con experiencia de más de 3 años con varios cursos que me certificaron por mis capacidades laborales.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutMe'
}
</script>

<style scoped>
.about-section {
  padding: 60px;
  background-color: #f7f7f7; /* Fondo suave para la sección */
}

.about-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1); 
  padding: 30px;
  overflow: hidden;
}

.about-img-container {
  flex: 1;
  padding-right: 20px; 
}

.about-img { 
  width: 200px;   
  height: 200px;  
  object-fit: cover;  
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1); 
}

.about-info {
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  flex: 2;
  font-size: 1.1em;
  color: #666;
  text-align: left; /* Alineación del texto */
}

.about-info h2 {
  font-size: 2em;
  margin-bottom: 20px;
  color: #333;
}

.about-info p {
  line-height: 1.6;
}

@media (max-width: 768px) {
  .about-container {
    flex-direction: column; 
    text-align: center;
  }

  .about-img-container {
    padding-right: 0;
    margin-bottom: 20px; /* Espacio debajo de la imagen */
  }

  .about-img {
    width: 150px;
    height: 150px;
  }

  .about-info {
    font-size: 1em;
  }
}
</style>
