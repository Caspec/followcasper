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
        <h2 class="text-white front-car-heading">Full Stack Web Development</h2>
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
        <h2 class="text-white front-car-heading">Cloud - CMS - Server setup - UX and more...</h2>
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
        <b-col class="front-content">
          <img class="img-fluid pb-3 mb-2 shadow" :src="require('../assets/dot1x200w.png')" alt="dot" title="Frontend Development" />
          <h3>Frontend Development</h3>
          <p>Responsive websites built for an optimal user experience that achieves your business goals.</p>
        </b-col>
        <b-col class="front-content">
          <img class="img-fluid pb-3 mb-2 shadow" :src="require('../assets/dot2x200w.png')" alt="dot" title="Full Stack Development" />
          <h3>Full Stack Development</h3>
          <p>Systems to be integrated together on different platforms and systems.</p>
        </b-col>
        <b-col class="front-content">
          <img class="img-fluid pb-3 mb-2 shadow" :src="require('../assets/dot3x200w.png')" alt="dot" title="CMS Development" />
          <h3>CMS Development</h3>
          <p>Manage your content using the web's most popular content management systems.</p>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="mt-4 mb-4">
      <b-row>
        <b-col>
        <div class="typical-wrap p-4 mb-4 shadow">
          <typical class="typicalWrapper font-weight-bold" :steps="['Welcome to my playground! 👋. Im currently available for a new job. 🚀', 4000, 'Im currently working on a real estate solution with Vue, Strapi and MySQL. 🚀', 4000, 'Fun fact - There are three species of zebra. 🦓', 4000, 'Fun fact - A lion’s roar can be heard from 5 miles away. 🦁', 4000, 'Fun fact - A crocodile can’t poke its tongue out. 🐊', 4000]" :loop="Infinity" :wrapper="'h3'"></typical>
        </div>
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
        <b-col><h2>Real Estate Commerce 24</h2></b-col>
      </b-row>
      <b-row>
        <b-col><h5>published 21 january 2021</h5></b-col>
      </b-row>
      <b-row>
        <b-col>
          <img class="img-fluid mb-3 shadow bg-white" :src="require('../assets/realestatecommerce24.jpg')" alt="Real Estate Commerce 24" title="Real Estate Commerce 24" />
          <p>I am currently in the process of developing a real estate site. It is developed in Vue, Strapi.js and with a MySQL database. I think it's great that Strapi.js and other similar headless CMS platforms can provide so much out of the box so you can focus on other things in the development phase than changing API routes in Node.js, relationships between tables in the database, small fixes and errors. Checkout <a href="https://strapi.io" target="_blank">Strapi headless CMS.</a></p>
          <p>I do not see anything else that headless CMS for many companies in the future will be the right way to go if they e.g. will make a Single Page Application with less maintenance and development hours so they could spend those hours improving the frontend optimization so the user gets a better experience of their website or mobile app.</p>
          <p>It depends of many things... as always in software development but I think companies will see the opportunities that it gives for their future web products or mobile products with use of headless CMS platforms. Checkout <a href="https://github.com/Caspec/real-estate-commerce-24" target="_blank">Real Estate Commerce 24 Github repo.</a></p>
          <p>Happy coding. <img class="img-fluid pb-1" :src="require('../assets/c.png')" alt="C" title="C" /></p>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row mt-4">
      <b-row>
        <b-col><h2>Website is live... <img class="img-fluid" :src="require('../assets/green.png')" alt="Live" title="Live" /></h2></b-col>
      </b-row>
      <b-row>
        <b-col><h5>published 09 november 2020</h5></b-col>
      </b-row>
      <b-row>
        <b-col>
          <img class="img-fluid mb-3 shadow bg-white" :src="require('../assets/newwebsite.png')" alt="New website" title="New website" />
          <p>Super cool that I got this site up and running. My next project is under way and I can reveal that it has something with the real-estate area.</p>
          <p>Happy coding. <img class="img-fluid pb-1" :src="require('../assets/c.png')" alt="C" title="C" /></p>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import typical from 'vue-typical'
export default {
  name: "Home",
  components: {
    typical
    },
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
  .front-content {
    margin-bottom: 2em;
  }
  .typical-wrap{
    margin: 0rem 0rem 0rem 0rem !important;
  }
  .typicalWrapper{
    font-size: 1.5rem;
  }
}

@media screen and (min-width: 767px) {
  .typical-wrap{
    margin: 2rem 0rem 0rem 0rem !important;
  }
}

@media screen and (max-width: 910px) {
.front-car-heading {
  font-size: 1.5rem !important;
}
}

.typicalWrapper::after {
  content: "|";
  animation: blink 1s infinite step-start;
  color: #2c8fd1;
}

@keyframes blink {
  50% { opacity: 0; }
}

</style>
