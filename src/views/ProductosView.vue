<template>

  <section class="container" id="productos">
  <h1 class=" text-center">Nuestros Productos</h1>
  <div class="row">
   
    <div class="col-sm-4 col-12 px-5 mb-4">

      <div class="card">
        <img src="../assets/img/colaciones.jpg" class="card-img-top" alt="colaciones" />
        <div class="card-body">
          <h5 class="card-title fw-bold">{{ nombre }}</h5>
          <p class="card-text">
            {{ descripcion }}
          </p>
        </div>
        <ul class="list-group list-group-flush">
          <li class="list-group-item">{{ cantidad }}</li>
          <li class="list-group-item">{{ precio }}</li>
        </ul>
        <div class="card-body">
          <a href="#" class="card-link">Ver más</a>
          <a href="#" class="card-link">Comprar</a>
        </div>
      </div>
    </div>
  </div>
</section>

  <router-link class="volver" to="/">Volver a Inicio</router-link>
</template>

<script>
export default {
  props: {
      nombre: {
          type: String,
          required: true
      },
      descripcion: {

          type: String,
          required: true
      },  
      cantidad: {
          type: String,
          required: true
      },
      precio: {
          type: String,
          required: true,
      },
  },
};
</script>


