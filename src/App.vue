<template>
  <div>
    <Navbar></Navbar>
    <div>
      <router-view />
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Footer from "./components/Footer";

export default {
  components: {
    Navbar,
    Footer
  }
};
</script>

<style>
 @import './css/style.css';
</style>
