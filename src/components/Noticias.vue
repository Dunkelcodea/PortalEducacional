<template>
  <div class="pt-3">
    
    <Noticia/>
    <Noticia/>
    <Noticia/>
    <Noticia/>
    <Noticia/>
    <Noticia/>
    <Noticia/>
  </div>
</template>

<script>
// @ is an alias to /src
import Noticia from '@/components/Noticia.vue'

export default {
  name: 'noticias',
  components: {
    Noticia
  }
}
</script>