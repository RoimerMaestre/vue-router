<template>
  <section class="hero">
    <div class="content">
      <h1>Bienvenido a Nuestra Página</h1>
      <p>Explora nuestros productos y servicios.</p>
      <div class="buttons">
        <router-link to="/producto">
          <button class="btn primary">Ver Productos</button>
        </router-link>
        <router-link to="/contacto">
          <button class="btn secondary">Contáctanos</button>
        </router-link>
      </div>
    </div>
    <div class="image">
      <img
        src="https://www.pequerecetas.com/wp-content/uploads/2021/03/comidas-rapidas.jpg"
        alt="Imagen de bienvenida"
      />
    </div>
  </section>
</template>

<script>
export default {
  name: "HomeView",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap");

body {
  font-family: "Montserrat", sans-serif;
  background-color: #f4f4f4;
  color: #333;
  margin: 0;
  padding: 0;
}

.hero {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 100px;

  color: #7f8c8d;
  height: 100vh;
}

.hero .content {
  max-width: 50%;
}

.hero h1 {
  font-size: 4rem;
  margin-bottom: 20px;
}

.hero p {
  font-size: 1.5rem;
  margin-bottom: 30px;
}

.hero .buttons {
  display: flex;
  gap: 20px;
}

.hero .btn {
  padding: 15px 30px;
  font-size: 1rem;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

.hero .btn.primary {
  background-color: #2ecc71;
  color: white;
}

.hero .btn.secondary {
  background-color: white;
  color: #3498db;
  border: 1px solid #3498db;
}

.hero .btn.primary:hover {
  background-color: #27ae60;
}

.hero .btn.secondary:hover {
  background-color: #b1bdc5;
  color: white;
  border-color: #3498db;
}

.hero .image img {
  max-width: 600px;
  border-radius: 10px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}

.hero .content,
.hero .image {
  max-width: 100%;
}

.hero .image img {
  width: 85%;
  max-width: 100%;
}
</style>
