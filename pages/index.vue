<template>
  <div>
<!--    <div class="loader">-->
<!--      <div class="lds-ripple">-->
<!--        <div></div>-->
<!--        <div></div>-->
<!--      </div>-->
<!--      <p class="text-center" style="color: #B7B4B9">the site may be a bit slow for the first time due to the number of high-quality images please be patient-->
<!--        :)</p>-->
<!--    </div>-->
    <div class="header">
      <b-container style="height: 100%" class="d-flex flex-column justify-content-center align-items-start">
        <b-row>
          <b-col md="12">
            <h1 class="main-headline mb-5">
              Hi, I'm Omar Jakmira,
              <a class="position-relative throw-line">a Full Stack Developer</a>
            </h1>
            <p class="about-me mb-5">
              I build high-quality mobile and web applications for businesses and individuals around the globe. if you
              need a modern and powerful website send me an email
            </p>
            <button @click="scrollToMyWork" class="main-btn main-btn-lg">see my work</button>
          </b-col>
        </b-row>
      </b-container>
    </div>

    <section class="work-gallery">
      <b-container>

        <!--        menhag-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Work In Progress</div>
                <h2 class="work-title">Learn Arabic With Menhag</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Laravel</span>
                  <span class="badge badge-light">Vuejs</span>
                  <span class="badge badge-light">MySql</span>
                </div>
                <div class="work-description">
                  This is Menhag a website intended for students who want to learn Arabic
                  the project is built with laravel 8 and vuejs 3
                  <br>
                  the admin panel is in laravel and blade and the rest of the project build as API/Client
                </div>

                <nuxt-link to="/projects/menhag" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head" src="/images/portfolio/menhag/1.jpg" alt="">
                  <img class="work-image-tail" src="/images/portfolio/menhag/2.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
          </b-row>

        </div>

        <!--        facebook clone-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Project for fun</div>
                <h2 class="work-title">Facebook clone</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Laravel</span>
                  <span class="badge badge-light">Vuejs</span>
                  <span class="badge badge-light">TDD</span>
                  <span class="badge badge-light">MySql</span>
                </div>
                <div class="work-description">
                  This is a small Facebook clone built while I'm learning vuejs and laravel TDD
                </div>

                <nuxt-link to="/projects/facebook_clone" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head" src="/images/portfolio/facebook/3.jpg" alt="">
                  <img class="work-image-tail" src="/images/portfolio/facebook/4.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
          </b-row>

        </div>

        <!--        dribbble clone-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Project for fun</div>
                <h2 class="work-title">Dribbble clone</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Laravel</span>
                  <span class="badge badge-light">Vuejs</span>
                  <span class="badge badge-light">Nuxt</span>
                  <span class="badge badge-light">MySql</span>
                </div>
                <div class="work-description">
                  This is a small Dribbble clone built while I'm learning vuejs and nuxt
                </div>

                <nuxt-link to="/projects/dribbble_clone" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head-big" src="/images/portfolio/dribble/1.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
          </b-row>

        </div>

        <!--        sawah-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Latest Work</div>
                <h2 class="work-title">Sawah</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Xamarin</span>
                  <span class="badge badge-light">C#</span>
                </div>
                <div class="work-description">
                  Sawah is an application for travel
                </div>

                <nuxt-link to="/projects/mobile/sawah" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head" src="/images/portfolio/sawah/1.jpg" alt="">
                  <img class="work-image-tail" src="/images/portfolio/sawah/4.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
          </b-row>

        </div>

        <!--        dealz-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Latest Work</div>
                <h2 class="work-title">Dealz</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Laravel</span>
                  <span class="badge badge-light">jQuery</span>
                  <span class="badge badge-light">MySql</span>
                </div>
                <div class="work-description">
                  Dealz is an open market for selling and bartering electrical devices
                  <br/>
                  with beautiful an easy to use UI
                </div>

                <nuxt-link to="/projects/dealz" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head" src="/images/portfolio/dealz/1.jpg" alt="">
                  <img class="work-image-tail" src="/images/portfolio/dealz/6.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
          </b-row>

        </div>

        <!--        kodwa-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Latest Work</div>
                <h2 class="work-title">Kodwa</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Laravel</span>
                  <span class="badge badge-light">jQuery</span>
                  <span class="badge badge-light">MySql</span>
                </div>
                <div class="work-description">
                  Kodwa is a small social network between students and their role models
                  <br/>
                  with beautiful an easy to use UI
                </div>

                <nuxt-link to="/projects/kodwa" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head" src="/images/portfolio/kodwa/1.jpg" alt="">
                  <img class="work-image-tail" src="/images/portfolio/kodwa/10.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
          </b-row>

        </div>

        <!--        food recipes-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Project for fun</div>
                <h2 class="work-title">Food Recipes</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Android</span>
                  <span class="badge badge-light">Kotlin</span>
                  <span class="badge badge-light">Jetpack</span>
                </div>
                <div class="work-description">
                  a native mobile application that I built while learning android jetpack
                  <br>
                  I used kotlin, HILT, Coroutines, and jetpack libraries like ROOM, ViewModel, and others
                </div>

                <nuxt-link to="/projects/mobile/recipes" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head" src="/images/portfolio/recipes/1.jpg" alt="">
                  <img class="work-image-tail" src="/images/portfolio/recipes/4.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
          </b-row>

        </div>

        <!--        resalati-->
        <div class="work">
          <b-row>
            <b-col md="6" sm="12">
              <div class="work-left">
                <div class="work-label">Latest Work</div>
                <h2 class="work-title">Resalati</h2>
                <div class="tags-container">
                  <span class="badge badge-light">Flutter</span>
                  <span class="badge badge-light">Android</span>
                  <span class="badge badge-light">IOS</span>
                </div>
                <div class="work-description">
                  Resalati is a social app that will send you a message every day that contain some information from
                  channels that you subscribed to it
                  <br>
                  Resalati built with flutter and Bloc provider for state management
                </div>

                <nuxt-link to="/projects/mobile/resalati" class="main-btn mt-5">see this project</nuxt-link>
              </div>
            </b-col>
            <b-col md="6" sm="12">
              <div class="work-right">
                <div class="work-images-wrapper">
                  <img class="work-image-head" src="/images/portfolio/resalati/20.jpg" alt="">
                  <img class="work-image-tail" src="/images/portfolio/resalati/1.jpg" alt="">
                </div>
                <img class="work-pattern" src="~/assets/images/dot.svg"/>
              </div>
            </b-col>
            <b-col md="12" class="d-flex justify-content-center big-top-margin">
              <button class="main-btn" @click="viewMore" v-if="!more">See more</button>
            </b-col>
          </b-row>

        </div>


        <template v-if="more">
          <!--          lara blog-->
          <div id="more" class="work">
            <b-row>
              <b-col md="6" sm="12">
                <div class="work-left">
                  <div class="work-label">Project For Fun</div>
                  <h2 class="work-title">LaraBlog</h2>
                  <div class="tags-container">
                    <span class="badge badge-light">Laravel</span>
                    <span class="badge badge-light">jQuery</span>
                    <span class="badge badge-light">MySql</span>
                  </div>
                  <div class="work-description">
                    LaraBlog is a simple website for blogging built with minimal UI
                  </div>

                  <nuxt-link to="/projects/lara_blog" class="main-btn mt-5">see this project</nuxt-link>
                </div>
              </b-col>
              <b-col md="6" sm="12">
                <div class="work-right">
                  <div class="work-images-wrapper">
                    <img class="work-image-head" src="/images/portfolio/laraBlog/2.png" alt="">
                    <img class="work-image-tail" src="/images/portfolio/laraBlog/1.png" alt="">
                  </div>
                  <img class="work-pattern" src="~/assets/images/dot.svg"/>
                </div>
              </b-col>
            </b-row>

          </div>
          <!--          rasheed crm-->
          <div class="work">
            <b-row>
              <b-col md="6" sm="12">
                <div class="work-left">
                  <div class="work-label">Latest Work</div>
                  <h2 class="work-title">Rasheed CRM</h2>
                  <div class="tags-container">
                    <span class="badge badge-light">Laravel</span>
                    <span class="badge badge-light">ElectronJs</span>
                    <span class="badge badge-light">ReacJs</span>
                    <span class="badge badge-light">Redux</span>
                    <span class="badge badge-light">MySql</span>
                  </div>
                  <div class="work-description">
                    Rasheed CRM is a CRM Desktop application built with web technologies
                  </div>

                  <nuxt-link to="/projects/rasheed" class="main-btn mt-5">see this project</nuxt-link>
                </div>
              </b-col>
              <b-col md="6" sm="12">
                <div class="work-right">
                  <div class="work-images-wrapper">
                    <img class="work-image-head-big" src="/images/portfolio/rasheed/1.jpg" alt="">
                  </div>
                  <img class="work-pattern" src="~/assets/images/dot.svg"/>
                </div>
              </b-col>
            </b-row>

          </div>
          <!--          aqare-->
          <div class="work">
            <b-row>
              <b-col md="6" sm="12">
                <div class="work-left">
                  <div class="work-label">Project for fun</div>
                  <h2 class="work-title">Aqare</h2>
                  <div class="tags-container">
                    <span class="badge badge-light">Laravel</span>
                    <span class="badge badge-light">Flutter</span>
                    <span class="badge badge-light">MySql</span>
                  </div>
                  <div class="work-description">
                    Aqare is a Cross-platform mobile application for real-estate
                    <br>
                    built with laravel and flutter and Bloc pattern for state management
                  </div>

                  <nuxt-link to="/projects/mobile/aqare" class="main-btn mt-5">see this project</nuxt-link>
                </div>
              </b-col>
              <b-col md="6" sm="12">
                <div class="work-right">
                  <div class="work-images-wrapper">
                    <img class="work-image-head" src="/images/portfolio/aqare/10.jpg" alt="">
                    <img class="work-image-tail" src="/images/portfolio/aqare/8.jpg" alt="">
                  </div>
                  <img class="work-pattern" src="~/assets/images/dot.svg"/>
                </div>
              </b-col>
            </b-row>

          </div>
          <!--          katebon-->
          <div class="work">
            <b-row>
              <b-col md="6" sm="12">
                <div class="work-left">
                  <div class="work-label">Latest Work</div>
                  <h2 class="work-title">Katebon</h2>
                  <div class="tags-container">
                    <span class="badge badge-light">Laravel</span>
                    <span class="badge badge-light">jQuery</span>
                    <span class="badge badge-light">MySql</span>
                  </div>
                  <div class="work-description">
                    Katebon is a Blogging Web application built with laravel
                  </div>

                  <nuxt-link to="/projects/katebon" class="main-btn mt-5">see this project</nuxt-link>
                </div>
              </b-col>
              <b-col md="6" sm="12">
                <div class="work-right">
                  <div class="work-images-wrapper">
                    <img class="work-image-head" src="/images/portfolio/katebon/4.jpg" alt="">
                    <img class="work-image-tail" src="/images/portfolio/katebon/2.jpg" alt="">
                  </div>
                  <img class="work-pattern" src="~/assets/images/dot.svg"/>
                </div>
              </b-col>
            </b-row>

          </div>
          <!--          rasheed_win-->
          <div class="work">
            <b-row>
              <b-col md="6" sm="12">
                <div class="work-left">
                  <div class="work-label">Old Work</div>
                  <h2 class="work-title">Rasheed Winforms</h2>
                  <div class="tags-container">
                    <span class="badge badge-light">VB.Net</span>
                    <span class="badge badge-light">windows forms</span>
                    <span class="badge badge-light">access</span>
                  </div>
                  <div class="work-description">
                    This is my first complete desktop application for Rasheed charity
                    <br/>
                    I built it in 2015 using visual basic .net
                  </div>

                  <nuxt-link to="/projects/rasheed_win" class="main-btn mt-5">see this project</nuxt-link>
                </div>
              </b-col>
              <b-col md="6" sm="12">
                <div class="work-right">
                  <div class="work-images-wrapper">
                    <img class="work-image-head-big" src="/images/portfolio/rasheed_winform/6.jpg" alt="">
                  </div>
                  <img class="work-pattern" src="~/assets/images/dot.svg"/>
                </div>
              </b-col>
            </b-row>

          </div>
        </template>

        <div class="what-i-do">
          <b-row>
            <b-col md="6">
              <h1>What <a class="throw-line">I do</a></h1>
            </b-col>
            <b-col md="6">
              <section class="ido-section">
                <h3>Web Development</h3>
                <p>
                  I build websites in multiple languages and frameworks like Laravel, NodeJs, Asp.net Core
                  I can also develop the front-end using Angular, Vue, and React
                </p>
              </section>
              <section class="ido-section">
                <h3>Mobile Development</h3>
                <p>
                  I can build cross-platform mobile applications using flutter and React Native
                  also, I have some experience in native development for android including kotlin and android jetpack
                </p>
              </section>
            </b-col>
          </b-row>
        </div>

      </b-container>
    </section>


  </div>
</template>

<script>
export default {
  layout: 'index',
  // created() {
  //   window.addEventListener('load', () => {
  //     setTimeout(() => {
  //       document.querySelector('.loader').remove()
  //       document.querySelector('body').style.overflow = 'auto'
  //     }, 500)
  //   })
  // },
  data() {
    return {
      more: false
    }
  },
  methods: {
    scrollToMyWork() {
      window.scrollTo({top: document.querySelector('.work-gallery').offsetTop - 30, behavior: 'smooth'})
    },
    viewMore() {
      this.more = !this.more
      setTimeout(() => {
        window.scrollTo({top: document.querySelector('#more').offsetTop - 30, behavior: 'smooth'})
      }, 200)
    }
  }
}
</script>

<style scoped>
body {
  overflow: hidden;
}
</style>
