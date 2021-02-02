<template>
<div>
  <div class="header">
    <b-container style="height: 100%" class="d-flex flex-column justify-content-center">
      <b-row>
        <b-col md="2"></b-col>
        <b-col md="8"  class="text-center">
          <p class="secondary-text">PROJECT SHOWCASE</p>
          <h1 class="main-headline mb-5">Aqare App</h1>
          <p class="description mb-5">
            Aqare is a Cross-platform mobile application for real-estate
            built with laravel and flutter
            <br> note: you can click the image to play the gallery
          </p>
        </b-col>
        <b-col md="2"></b-col>
      </b-row>
    </b-container>
  </div>
  <b-container>
    <b-row>
      <b-col md="12">
        <div class="project-main-image-mobile">
          <img @click="changeImage" ref="mainImage" :src="images[selectedImage]" alt="">
        </div>

      </b-col>
    </b-row>
  </b-container>
</div>
</template>

<script>
export default {
name: "menhag",
  data(){
  return {
    selectedImage:0,
    images:[
      '/images/portfolio/aqare/1.jpg',
      '/images/portfolio/aqare/2.jpg',
      '/images/portfolio/aqare/3.jpg',
      '/images/portfolio/aqare/4.jpg',
      '/images/portfolio/aqare/5.jpg',
      '/images/portfolio/aqare/6.jpg',
      '/images/portfolio/aqare/7.jpg',
      '/images/portfolio/aqare/8.jpg',
      '/images/portfolio/aqare/9.jpg',
      '/images/portfolio/aqare/10.jpg',
      '/images/portfolio/aqare/11.jpg',
      '/images/portfolio/aqare/12.jpg',
      '/images/portfolio/aqare/13.jpg',
      '/images/portfolio/aqare/14.jpg',
      '/images/portfolio/aqare/15.jpg'
    ]
  }
  },
  methods:{
    changeImage(){
      if (this.selectedImage >= this.images.length -1){
        this.selectedImage = 0
      }

      this.$refs.mainImage.src = this.images[++this.selectedImage]
      window.scrollTo({top:document.querySelector('img').offsetTop + 900,behavior:'smooth'});

    }
  }

}
</script>

<style scoped>

</style>
