<template>
  <section class="container" id="productos">
    <div class="row">
      <Card
        v-bind:nombre="nombre"
        v-bind:descripcion="descripcion"
        v-bind:precio="precio"
        v-bind:cantidad="cantidad"
      />
    </div>
  </section>
</template>

<script>
import Card from "@/components/Card.vue";
export default {
  name: "ProductoView",
  components: {
    Card,
  },
  props: {
    nombre: String,
    descripcion: String,
    precio: String,
    cantidad: String,
  },
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
h2 {
  margin: 200px;
}
</style>
