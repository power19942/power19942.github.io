<template>
<div>
  <div class="header">
    <b-container style="height: 100%" class="d-flex flex-column justify-content-center">
      <b-row>
        <b-col md="2"></b-col>
        <b-col md="8"  class="text-center">
          <p class="secondary-text">PROJECT SHOWCASE</p>
          <h1 class="main-headline mb-5">Resalati App</h1>
          <p class="description mb-5">
            Resalati is a social app that will send you message every day that contain some information from channels that you subscribed to it
            Resalati built with flutter and Bloc pattern for state management
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
      '/images/portfolio/resalati/1.jpg',
      '/images/portfolio/resalati/2.jpg',
      '/images/portfolio/resalati/3.jpg',
      '/images/portfolio/resalati/4.jpg',
      '/images/portfolio/resalati/5.jpg',
      '/images/portfolio/resalati/6.jpg',
      '/images/portfolio/resalati/7.jpg',
      '/images/portfolio/resalati/8.jpg',
      '/images/portfolio/resalati/9.jpg',
      '/images/portfolio/resalati/10.jpg',
      '/images/portfolio/resalati/11.jpg',
      '/images/portfolio/resalati/12.jpg',
      '/images/portfolio/resalati/13.jpg',
      '/images/portfolio/resalati/14.jpg',
      '/images/portfolio/resalati/15.jpg',
      '/images/portfolio/resalati/16.jpg',
      '/images/portfolio/resalati/17.jpg',
      '/images/portfolio/resalati/18.jpg',
      '/images/portfolio/resalati/19.jpg',
      '/images/portfolio/resalati/20.jpg',
      '/images/portfolio/resalati/21.jpg',
      '/images/portfolio/resalati/22.jpg',
      '/images/portfolio/resalati/23.jpg',
      '/images/portfolio/resalati/24.jpg',
      '/images/portfolio/resalati/25.jpg',
      '/images/portfolio/resalati/26.jpg',
      '/images/portfolio/resalati/27.jpg',
      '/images/portfolio/resalati/28.jpg',
      '/images/portfolio/resalati/29.jpg',
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
