<template>
  <div>
    <b-navbar type="dark" variant="dark">
      <b-navbar-nav>
        <b-nav-item :to="{ name: 'Home'}"><b-icon icon="house-fill" variant="success"></b-icon> Home</b-nav-item>
        <b-nav-item :to="{ name: 'About'}"><b-icon icon="card-text" variant="info"></b-icon> About</b-nav-item>
      </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<script>
export default {

};
</script>

<style scoped>

</style>