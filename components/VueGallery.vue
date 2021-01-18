<template>
  <b-row align-v="stretch">
    <gallery :images="images" :index="index" @close="index = null" />
    <b-col
      v-for="(image, imageIndex) in images"
      :key="imageIndex"
      cols="4"
      class="image"
      :style="{
        backgroundImage: 'url(' + image + ')',
        width: '300px',
        height: '200px',
      }"
      @click="index = imageIndex"
    />
  </b-row>
</template>

<script>
import VueGallery from 'vue-gallery'

export default {
  components: {
    gallery: VueGallery
  },
  data () {
    return {
      images: [
        'https://picsum.photos/400',
        'https://picsum.photos/800',
        'https://picsum.photos/1200',
        'https://picsum.photos/1600',
        'https://picsum.photos/2000',
        'https://picsum.photos/2400'
      ],
      index: null
    }
  }
}
</script>

<style scoped>
.image {
  float: left;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  border: 1px solid #ebebeb;
  margin: 50px auto;
}
</style>
