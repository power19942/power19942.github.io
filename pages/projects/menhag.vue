<template>
<div>
  <div class="header">
    <b-container style="height: 100%" class="d-flex flex-column justify-content-center">
      <b-row>
        <b-col md="2"></b-col>
        <b-col md="8"  class="text-center">
          <p class="secondary-text">PROJECT SHOWCASE</p>
          <h1 class="main-headline mb-5">Menhag Website</h1>
          <p class="description mb-5">
            Menhag is a platform for learning arabic language
            built with laravel and vuejs
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
        <div class="project-main-image">
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
      '/images/portfolio/menhag/1.png',
      '/images/portfolio/menhag/2.png',
      '/images/portfolio/menhag/3.png',
      '/images/portfolio/menhag/4.png',
      '/images/portfolio/menhag/5.png',
      '/images/portfolio/menhag/6.png',
      '/images/portfolio/menhag/7.png',
      '/images/portfolio/menhag/8.png',
      '/images/portfolio/menhag/9.png',
      '/images/portfolio/menhag/10.png',
      '/images/portfolio/menhag/11.png',
      '/images/portfolio/menhag/12.png',
      '/images/portfolio/menhag/13.png',
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
