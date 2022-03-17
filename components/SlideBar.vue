<template>
       <div class="mb-2" id="carousel">
            <b-carousel
                id="carousel-fade"
                style="text-shadow: 0px 0px 2px #000"
                fade
                indicators
                img-width="1024"
                img-height="580"
            >
                <b-carousel-slide v-for="(image, index) in images" :key="index"
                :img-src="image.src"
                ></b-carousel-slide>
            </b-carousel>
        </div>
</template>

<script>
  export default {
      props: {
          images: Array,
      },
      data() {
          return {
              
          }
      },
      computed: {
          test() {
                console.log(this.images);
          }
          
      }
  }
</script>