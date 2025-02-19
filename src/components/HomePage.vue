<template>
  <div id="home" class="home-section">
    <h1>Bienvenido a mi Portfolio</h1>
    <p>Estudiante de Programacion y Gte Turno</p>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
}
</script>

<style scoped>
.home-section {
  font-family: 'Times New Roman', Times, serif;
  text-align: center;
  padding: 60px;
  background-color: #f7f7f7;
  margin-top: 0; /* Elimina margen superior */
}

.home-section h1 {
  font-size: 3em;
  margin-bottom: 20px;
}

.home-section p {
  font-size: 1.2em;
  color: #333;
}
</style>
