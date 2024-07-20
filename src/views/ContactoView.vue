<template>
  <div class="contact-container">
    <h2>Contacto</h2>
    <div class="contact-form">
      <form>
        <div class="form-group">
          <label for="name">Nombre</label>
          <input type="text" id="name" placeholder="Tu nombre" />
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" placeholder="Tu email" />
        </div>
        <div class="form-group">
          <label for="message">Mensaje</label>
          <textarea id="message" rows="4" placeholder="Tu mensaje"></textarea>
        </div>
        <button type="submit" class="submit-btn">Enviar</button>
      </form>
    </div>
    <div class="social-media">
      <a href="#" class="social-icon"><i class="fab fa-facebook-f"></i></a>
      <a href="#" class="social-icon"><i class="fab fa-twitter"></i></a>
      <a href="#" class="social-icon"><i class="fab fa-instagram"></i></a>
      <a href="#" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
    </div>
    <router-link to="/"> <a href="" class="home-btn">Inicio</a></router-link>
    
  </div>
</template>

<script>
export default {
  name: 'ContactoView',
};
</script>

<style scoped>
.contact-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 50px 20px;
  background: #f9f9f9;
  border-radius: 10px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  margin-top: 5rem;
}

h2 {
  font-size: 2.5rem;
  color: #333;
  margin-bottom: 20px;
}

.contact-form {
  width: 100%;
  max-width: 600px;
  background: #fff;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
  margin-bottom: 30px;
}

.form-group {
  margin-bottom: 15px;
}

.form-group label {
  display: block;
  font-size: 1rem;
  color: #666;
  margin-bottom: 5px;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 1rem;
}

.form-group input:focus,
.form-group textarea:focus {
  outline: none;
  border-color: #007bff;
}

.submit-btn {
  display: inline-block;
  background: #007bff;
  color: #fff;
  padding: 10px 20px;
  font-size: 1rem;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background 0.3s;
}

.submit-btn:hover {
  background: #0056b3;
}

.social-media {
  display: flex;
  justify-content: center;
  gap: 20px;
}

.social-icon {
  font-size: 1.5rem;
  color: #007bff;
  transition: color 0.3s;
}

.social-icon:hover {
  color: #0056b3;
}

.home-btn {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 20px;
  background: #28a745;
  color: #fff;
  text-decoration: none;
  font-size: 1rem;
  border-radius: 5px;
  transition: background 0.3s;
}

.home-btn:hover {
  background: #218838;
}
</style>
