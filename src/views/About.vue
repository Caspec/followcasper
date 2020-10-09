<template>
  <div id="about">
    <b-container class="bv-row mt-3 pt-3 pb-3">
      <b-row>
        <b-col>
          <h1 class="mt-2">About me</h1>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <h3>Hi. I am Casper, a Full Stack Web Developer with a great interest in making websites and web applications.</h3>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <img class="img-fluid shadow bg-white" :src="require('../assets/me.png')" alt="Me" title="Me" />
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row mt-2 fluid">
      <b-row>
        <b-col>
          <h4>Download my <a href="./cv-casperENG.pdf" download="cv-casperENG.pdf">CV</a></h4>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row mt-2 fluid">
      <b-row>
        <b-col>
          <p>I work to make a better web; one that is fast, easy to use, beautiful, accessible to all, and frustration-free. Regardless of your specific business requirements, in solving these challenges, you have a great chance of finding success online.</p>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <p>My main experience is in Full Stack Development. Given that producing a modern website requires the combination of design, server technology, and the layer that users interacts with, I believe having experience in both design and development allows for making the most optimal user experiences.</p>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row fluid">
      <b-row>
        <b-col>
         <h4>Skill set</h4>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <ul class="list-unstyled mt-2">
            <li>
              <span class="font-weight-bold"><img class="img-fluid" :src="require('../assets/sourcex2.png')" alt="Source" title="Source" /> Full Stack Web Development</span>
            </li>
            <li class="pt-2">
              <span class="font-weight-bold"><img class="img-fluid" :src="require('../assets/vuex2.png')" alt="Vue" title="Vue" /> Vue</span>
            </li>
            <li class="pt-2">
              <span class="font-weight-bold"><img class="img-fluid" :src="require('../assets/reactx2.png')" alt="React" title="React" /> React</span>
            </li>
            <li class="pt-2">
              <span class="font-weight-bold"><img class="img-fluid" :src="require('../assets/javascriptx2.png')" alt="JS" title="JS" /> JS</span>
            </li>
            <li class="pt-2">
              <span class="font-weight-bold"><img class="img-fluid" :src="require('../assets/axx2.png')" alt="AX" title="AX" /> Accessibility</span>
            </li>
            <li class="pt-2">
              <span class="font-weight-bold"><img class="img-fluid" :src="require('../assets/morex2.png')" alt="More" title="More" /> More</span>
            </li>
          </ul>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {

};
</script>

<style scoped>

</style>