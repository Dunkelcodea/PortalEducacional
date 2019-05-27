<template>
  <div class="home">
    <b-row class="pt-1 pl-0">
    <b-col md="12" class="carru"><Carrusel></Carrusel></b-col>
    <b-col cols="12" md="8"><Noticias/></b-col>
    <b-col cols="12" md="4"><RedesSociales/></b-col>
    
  </b-row>
    
  </div>
</template>


<style>
@media (max-width: 600px) {
  .carru {
    display: none;
  }
}
</style>

<script>
// @ is an alias to /src
import Carrusel from '@/components/Carrusel.vue'
import Noticias from '@/components/Noticias.vue'
import RedesSociales from '@/components/RedesSociales.vue'

export default {
  name: 'home',
  components: {
    Carrusel,
    Noticias,
    RedesSociales
  }
}
</script>
