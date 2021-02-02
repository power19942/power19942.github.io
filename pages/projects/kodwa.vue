<template>
  <div>
    <div class="header">
      <b-container style="height: 100%" class="d-flex flex-column justify-content-center">
        <b-row>
          <b-col md="2"></b-col>
          <b-col md="8" class="text-center">
            <p class="secondary-text">PROJECT SHOWCASE</p>
            <h1 class="main-headline mb-5">Kodwa Website</h1>
            <p class="description mb-5">
              Kodwa is a small social network between students and their role models
              with beautiful an easy to use UI
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
  data() {
    return {
      selectedImage: 0,
      images: [
        '/images/portfolio/kodwa/1.jpg',
        '/images/portfolio/kodwa/2.jpg',
        '/images/portfolio/kodwa/3.jpg',
        '/images/portfolio/kodwa/4.jpg',
        '/images/portfolio/kodwa/5.jpg',
        '/images/portfolio/kodwa/6.jpg',
        '/images/portfolio/kodwa/7.jpg',
        '/images/portfolio/kodwa/8.jpg',
        '/images/portfolio/kodwa/9.jpg',
        '/images/portfolio/kodwa/10.jpg',
        '/images/portfolio/kodwa/11.jpg',
      ]
    }
  },
  methods: {
    changeImage() {
      if (this.selectedImage >= this.images.length - 1) {
        this.selectedImage = 0
      }

      this.$refs.mainImage.src = this.images[++this.selectedImage]
      window.scrollTo({top: document.querySelector('img').offsetTop + 900, behavior: 'smooth'});

    }
  }

}
</script>

<style scoped>

</style>
