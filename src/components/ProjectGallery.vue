<template>
  <div id="gallery" class="gallery-section">
    <h2>Galería de Proyectos</h2>
    <div class="projects">
      <div class="project">
        <img src="@/assets/project1.png" alt="Proyecto 1" class="project-img"/>
        <p>Creador de una pagina web para ventas de ropa de gimnasio</p>
      </div>
      <div class="project">
        <img src="@/assets/project2.png" alt="Proyecto 2" class="project-img"/>
        <p>Diseñador de la pagina Web de magicbook y database</p>
      </div>
      <div class="project">
        <img src="project3.jpg" alt="Proyecto 3" class="project-img"/>
        <p>Descripción del proyecto 3</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProjectGallery'
}
</script>

<style scoped>
.gallery-section {
  text-align: center;
  padding: 60px;
  background-color: #fafafa;
}

.gallery-section h2 {
  font-size: 2.5em;
  margin-bottom: 30px;
}

.projects {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
}

.project {
  width: 300px;
  background-color: #fff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease; /* Transición suave para el hover */
}

.project:hover {
  transform: scale(1.05); 
  box-shadow: 0px 10px 15px rgba(0, 0, 0, 0.2); 
}

.project-img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 20px;
}

.project p {
  font-size: 1em;
  color: #333;
}
</style>
