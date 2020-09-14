<template>
  <div class="home">
    <h1 class="mt-2 mb-2">home....</h1>
    <h4>bla bla bla</h4>
    <b-container class="bv-example-row">
      <b-row>
        <b-col>
          <div>
            <img class="img-fluid mt-2 mb-2" :src="require('../assets/herobig.png')" alt="Image" />
          </div>
        </b-col>
      </b-row>
    </b-container>

    <b-container fluid="md" class="mb-4">
      <b-row>
        <b-col>
          <h4>bla bla</h4>
          <h4>bla bla</h4>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
        bla bla bla bla bla bla bla bla bla bla bla bla
        </b-col>
      </b-row>
    </b-container>
    
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {

  }
};
</script>
