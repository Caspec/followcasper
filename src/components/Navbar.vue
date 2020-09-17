<template>
  <div class="nav">
    <b-container class="bv-row">
      <b-row class="text-left text-white">
        <b-col class="pt-3">
          <router-link to="/" class="logotext">followcasper</router-link>
        </b-col>
        <b-col cols="8">
          <b-navbar type="black" variant="black">
            <b-navbar-nav>
              <b-nav-item :to="{ name: 'Home'}">Home</b-nav-item>
              <!-- Navbar dropdowns -->
              <b-nav-item-dropdown text="Portfolio" center>
                <b-dropdown-item :to="{ name: 'About'}">About</b-dropdown-item>
                <b-dropdown-item href="#">2</b-dropdown-item>
                <b-dropdown-item href="#">3</b-dropdown-item>
                <b-dropdown-item href="#">4</b-dropdown-item>
              </b-nav-item-dropdown>

              <b-nav-item-dropdown text="User" left>
                <b-dropdown-item href="#">Account</b-dropdown-item>
                <b-dropdown-item href="#">Settings</b-dropdown-item>
              </b-nav-item-dropdown>
            </b-navbar-nav>
          </b-navbar>
        </b-col>
        <b-col class="text-center pt-3">
          <router-link to="/"><img class="img-fluid" :src="require('../assets/denmark-flag-icon-16.png')" alt="DK" /></router-link>
          <router-link to="/"><img class="img-fluid pl-2" :src="require('../assets/united-kingdom-flag-icon-16.png')" alt="ENG" /></router-link>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>

<style>

.nav {
  background-color: #000;
  padding: 10px;
}

.logotext {
  font-family: "Righteous", cursive;
  text-decoration: none;
  color: #fff;
}

.logotext:hover {
  text-decoration: none;
  color: #2c8fd1;
}

.dropdown-menu {
  background-color: rgb(0,0,0) !important;
  color: #fff !important;
  padding-top: 15px !important;
}

.dropdown-item {
  background-color: rgb(0,0,0) !important;
  color: #c4c4c4 !important;
  font-family: "Roboto", sans-serif;
}

.dropdown-item:hover {
  background-color: rgba(48, 48, 48, 0.79) !important;
  color: #a50101 !important;
}

.nav-link {
  color: #ff0000 !important;
  font-family: "Roboto", sans-serif;
}

.nav-link:hover {
  color: #a50101 !important;
}

</style>