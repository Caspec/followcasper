<template>
  <div class="home">
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      fade
      background="#ababab"
      img-width="600"
      img-height="100"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <b-carousel-slide>
        <template v-slot:img>
          <router-link to="/">
            <img
              class="d-block img-fluid w-100"
              width="1500"
              height="200"
              :src="require('../assets/slide1.png')"
              alt="slide"
            />
          </router-link>
        </template>
        <h2 class="text-white">Full Stack Web Development</h2>
      </b-carousel-slide>
      <b-carousel-slide>
        <template v-slot:img>
          <router-link to="/About">
            <img
              class="d-block img-fluid w-100"
              width="1500"
              height="200"
              :src="require('../assets/slide2.png')"
              alt="slide"
            />
          </router-link>
        </template>
        <h2 class="text-white">Cloud - CMS - Server setup - UX and more...</h2>
      </b-carousel-slide>
    </b-carousel>

    <b-container class="bv-row mt-3 pt-3 pb-3">
      <b-row>
        <b-col>
          <h1>Full Stack Web Developer</h1>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <h3>Hi. I am Casper, a Full Stack Web Developer with a great interest in making websites and web applications. Read more about me and what I do in the <router-link  to="/about">about section.</router-link></h3>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row mt-3 pt-4">
      <b-row>
        <b-col>
          <img class="img-fluid pb-3" :src="require('../assets/dot1x200w.png')" alt="dot" title="Frontend Development" />
          <h3>Frontend Development</h3>
          <p>Responsive websites built for an optimal user experience that achieves your business goals.</p>
        </b-col>
        <b-col>
          <img class="img-fluid pb-3" :src="require('../assets/dot2x200w.png')" alt="dot" title="Full Stack Development" />
          <h3>Full Stack Development</h3>
          <p>Systems to be integrated together on different platforms and systems.</p>
        </b-col>
        <b-col>
          <img class="img-fluid pb-3" :src="require('../assets/dot3x200w.png')" alt="dot" title="CMS Development" />
          <h3>CMS Development</h3>
          <p>Manage your content using the web's most popular content management systems.</p>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="mt-3" fluid>
      <b-row>
        <b-col>
          <hr >
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row mt-4">
      <b-row>
        <b-col><h2>Website is live... <img class="img-fluid" :src="require('../assets/green.png')" alt="Live" title="Live" /></h2></b-col>
      </b-row>
      <b-row>
        <b-col><h4>09-11-2020</h4></b-col>
      </b-row>
      <b-row>
        <b-col>
          <img class="img-fluid mb-3 shadow bg-white" :src="require('../assets/newwebsite.png')" alt="New website" title="New website" />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {},
  data() {
    return {
      slide: 0,
      sliding: null,
    };
  },
  methods: {
    onSlideStart() {
      this.sliding = true;
    },
    onSlideEnd() {
      this.sliding = false;
    },
  },
};
</script>

<style>
@media screen and (max-width: 767px) {
  #carousel-1 {
    display: none;
  }
}
</style>
