<template>
<div>
  <div class="header">
    <b-container style="height: 100%" class="d-flex flex-column justify-content-center">
      <b-row>
        <b-col md="2"></b-col>
        <b-col md="8"  class="text-center">
          <p class="secondary-text">PROJECT SHOWCASE</p>
          <h1 class="main-headline mb-5">Sawah App</h1>
          <p class="description mb-5">
            Sawah is an application for travel
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
      '/images/portfolio/sawah/1.jpg',
      '/images/portfolio/sawah/2.jpg',
      '/images/portfolio/sawah/3.jpg',
      '/images/portfolio/sawah/4.jpg',
      '/images/portfolio/sawah/5.jpg',
      '/images/portfolio/sawah/6.jpg',
      '/images/portfolio/sawah/7.jpg',
      '/images/portfolio/sawah/8.jpg',
      '/images/portfolio/sawah/9.jpg',
      '/images/portfolio/sawah/10.jpg',
      '/images/portfolio/sawah/11.jpg',
      '/images/portfolio/sawah/12.jpg',
      '/images/portfolio/sawah/13.jpg',
      '/images/portfolio/sawah/14.jpg',
      '/images/portfolio/sawah/15.jpg',
      '/images/portfolio/sawah/16.jpg',
      '/images/portfolio/sawah/17.jpg',
      '/images/portfolio/sawah/18.jpg',
      '/images/portfolio/sawah/19.jpg',
      '/images/portfolio/sawah/20.jpg',
      '/images/portfolio/sawah/21.jpg',
      '/images/portfolio/sawah/22.jpg',
      '/images/portfolio/sawah/23.jpg',
      '/images/portfolio/sawah/24.jpg',
      '/images/portfolio/sawah/25.jpg',
      '/images/portfolio/sawah/26.jpg',
      '/images/portfolio/sawah/27.jpg',
      '/images/portfolio/sawah/28.jpg',
      '/images/portfolio/sawah/29.jpg',
    ]
  }
  },
  methods:{
    changeImage(){
      if (this.selectedImage >= this.images.length -1){
        this.selectedImage = 0
      }

      this.$refs.mainImage.src = this.images[++this.selectedImage]
      //window.scrollTo({top:document.querySelector('img').offsetTop + 900,behavior:'smooth'});

    }
  }

}
</script>

<style scoped>

</style>
