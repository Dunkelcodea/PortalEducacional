<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="2000"
      controls
      indicators
      background="#ababab"
      
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="Bienvenido"
        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
        img-src="http://www.insertus.com/wp-content/uploads/2015/08/fotos-panoramicas-1.jpg"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="http://www.insertus.com/wp-content/uploads/2015/08/fotos-panoramicas-12.jpg">
        <h1>Portal Educativo</h1>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide img-src="http://gabrielroux.com.mx/wp-content/uploads/2013/01/panoramicas007.jpg"></b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <img
          slot="img"
          class="d-block img-fluid w-100"
          width="100%"
          height="70%"
          src="http://www.eolia.es/wp-content/uploads/2016/05/panoramica-cielo-nocturno-1.png"
          alt="image slot"
        >
      </b-carousel-slide>


    </b-carousel>

    <!-- <p class="mt-4">
      Slide #: {{ slide }}<br>
      Sliding: {{ sliding }}
    </p> -->
  </div>
</template>

<script>
  export default {
    data() {
      return {
        slide: 0,
        sliding: null,
        ancho:100,
        alto:200
      }
    },
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>