<template>
  <div id="contact" class="contact-section">
    <h2>Contacto</h2>
    <form>
      <div class="form-group">
        <label for="name">Nombre</label>
        <input type="text" class="form-control" id="name" placeholder="Ingresa tu nombre" />
      </div>
      <div class="form-group">
        <label for="email">Correo Electrónico</label>
        <input type="email" class="form-control" id="email" placeholder="Ingresa tu email" />
      </div>
      <div class="form-group">
        <label for="message">Mensaje</label>
        <textarea class="form-control" id="message" rows="3" placeholder="Escribe tu mensaje"></textarea>
      </div>
      <button type="submit" class="btn btn-primary">Enviar Mensaje</button>
    </form>

    <!-- Nueva sección debajo del formulario -->
    <div class="footer-section">
      <div class="footer-column">
        <h3>About us</h3>
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio doloremque porro
          molestias temporibus omnis.
        </p>
      </div>
      <div class="footer-column">
        <h3>Quick Links</h3>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About me</a></li>
          <li><a href="#gallery">Gallery</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
      <div class="footer-column">
        <h3>Contact</h3>
        <p>Email: carlosmartinezhdez445@gmail.com</p>
        <p>Phone: (984) 158 1553</p>
        <p>Adress: Playa del Carmen, MX</p>
      </div>
    </div>

    <!-- Copyright Section -->
    <div class="copyright-section">
      <p>© 2025 By Carlos Eduardo Martinez. All rights reserved.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactForm',
};
</script>

<style scoped>
.contact-section {
  padding: 60px;
  background-color: #f4f4f4;
}

.contact-section h2 {
  font-size: 2.5em;
  margin-bottom: 30px;
}

.form-group {
  margin-bottom: 20px;
}

.form-control {
  padding: 10px;
  width: 100%;
  border-radius: 5px;
}

.btn {
  margin-top: 20px;
  background-color: #007bff;
  border: none;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
}

.btn:hover {
  background-color: #0056b3;
}

/* Nueva sección de pie de página */
.footer-section {
  display: flex;
  justify-content: space-between;
  margin-top: 40px;
  background-color: #333;
  color: white;
  padding: 20px 60px;
  width: 100%; 
  box-sizing: border-box; 
}

.footer-column {
  width: 30%;
}

.footer-column h3 {
  font-size: 1.5em;
  margin-bottom: 10px;
}

.footer-column p,
.footer-column ul {
  font-size: 1em;
}

.footer-column ul {
  padding-left: 0;
}

.footer-column ul li {
  list-style: none;
}

.footer-column ul li a {
  color: white;
  text-decoration: none;
}

.footer-column ul li a:hover {
  text-decoration: underline;
}

/* Sección de copyright al final */
.copyright-section {
  background-color: #222;
  color: white;
  text-align: center;
  padding: 20px;
  margin-top: 0; /* Elimina el margen superior */
}

.copyright-section p {
  font-size: 1em;
  margin: 0;
}
/* Responsividad */
@media (max-width: 768px) {
  .footer-section {
    flex-direction: column;
    align-items: center;
  }
  .footer-column {
    width: 100%;
  }
  .contact-section {
    padding: 30px;
  }
  .contact-section h2 {
    font-size: 2em;
  }
}
</style>

