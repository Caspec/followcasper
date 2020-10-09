<template>
  <div id="contact">
    <b-container class="bv-row mt-3 pt-3 pb-3">
      <b-row>
        <b-col>
          <h1 class="mt-2">Contact me</h1>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <h3>Send a general message or details of a project you'd like me to be a part of and I'll get back to you as soon as possible.</h3>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row mt-2 fluid">
      <b-row>
        <b-col>
          <p>You can contact me through this form, enter your name, email and your message. I will strive to answer you as soon as possible.</p>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
          <p>You can read more about me on the <router-link  to="/about">about section</router-link> and otherwise you can read my <a href="./cv-casperENG.pdf" target="_blank">CV.</a></p>
        </b-col>
      </b-row>
    </b-container>

    <b-container class="bv-row mt-4">
    <form>
       <div class="form-group">
            <label for="name">Your name*</label>
            <input type="text" class="form-control" id="name" placeholder="Enter your name">
        </div>
        <div class="form-group">
            <label for="email">Email address*</label>
            <input type="email" class="form-control" id="email" placeholder="Enter your email">
        </div>
        <div class="form-group">
            <label for="textarea">General message*</label>
            <textarea class="form-control" id="textarea" rows="3" placeholder="Enter your message"></textarea>
        </div>
        <button type="submit" class="btn btn-primary">Send</button>
    </form>
    </b-container>
  </div>
</template>

<script>
export default {

};
</script>

<style scoped>

</style>