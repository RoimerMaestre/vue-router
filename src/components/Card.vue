<template>
  <!-- cartas -->
  <section class="container" id="productos">
    <h1 class="text-center">Nuestros Productos</h1>
    <div class="row">
      <!-- primera -->
      <div class="col-12 card-container">
        <div class="card">
          <img
            src="../assets/img/colaciones.jpg"
            class="card-img-top"
            alt="colaciones"
          />
          <div class="card-body">
            <h5 class="card-title">{{ nombre }}</h5>
            <p class="card-text">
              {{ descripcion }}
            </p>
          </div>
          <ul class="list-group">
            <li class="list-group-item">{{precio}}</li>
            <li class="list-group-item">{{cantidad}}</li>
          </ul>
          <div class="card-body">
            <a href="#" class="card-link button">Ver más</a>
            <a href="#" class="card-link button">Comprar</a>
          </div>
        </div>
      </div>
    </div>
    <router-link to="/"> <a href="#" id="inicio">Inicio</a></router-link>
  </section>
</template>

<script>
export default {
  name: "card",
  props: ["nombre", "descripcion", "precio", "cantidad"],
};
</script>

<style scoped>
.container {
  max-width: 25rem;
  margin: 0 auto;
  padding: 20px;
}

.text-center {
  text-align: center;
  font-family: "Arial", sans-serif;
}

.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.card-container {
  flex: 1 1 30%;
  margin: 10px;
  padding: 20px;
  box-sizing: border-box;
}

.card {
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s ease;
  background-color: #fff;
}

.card:hover {
  transform: translateY(-5px);
}

.card-img-top {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.card-body {
  padding: 15px;
  text-align: center;
}

.card-title {
  font-size: 1.25rem;
  margin-bottom: 10px;
  font-weight: bold;
}

.card-text {
  font-size: 1rem;
  margin-bottom: 15px;
  color: #555;
}

.list-group {
  list-style: none;
  padding: 0;
  margin: 0;
  border-top: 1px solid #ddd;
}

.list-group-item {
  padding: 10px;
  border-bottom: 1px solid #ddd;
}

.card-link {
  display: inline-block;
  margin: 10px 0;
  text-decoration: none;
  transition: background-color 0.3s ease, color 0.3s ease;
  margin: 10px;
}

.button {
  padding: 10px 20px;
  border-radius: 5px;
  background-color: #007bff;
  color: white;
}

.button:hover {
  background-color: #0056b3;
}

#inicio {
  display: block;
  margin-top: 20px;
  text-align: center;
  font-size: 1.1rem;
  border: 1px solid blue;
}
</style>
