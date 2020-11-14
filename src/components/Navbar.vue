<template>
  <div class="navbg shadow">
    <b-navbar toggleable="lg" type="dark" variant="black">
      <b-navbar-brand>
        <router-link
          to="/"
          class="logotext"
          title="Casper - Full Stack Web Developer"
          >followcasper</router-link
        >
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="nav-space">
          <b-nav-item :to="{ name: 'Home' }">Home</b-nav-item>
          <b-nav-item :to="{ name: 'About' }">About</b-nav-item>
          <b-nav-item-dropdown text="Portfolio">
            <b-dropdown-item
              href="https://picassoonline.techotel.dk/en/hestraviken/hotel/booking/rooms/"
              target="_blank"
              >Hestraviken Online booking</b-dropdown-item
            >
            <b-dropdown-item
              href="https://picassoonline.techotel.dk/en/kolding-hotel-apartments/kolding-hotel-apartments/booking/accommodation/"
              target="_blank"
              >Kolding Online booking</b-dropdown-item
            >
            <b-dropdown-item
              href="https://www.giftcard.followcasper.dk"
              target="_blank"
              >Giftcard project</b-dropdown-item
            >
            <b-dropdown-item
              href="https://github.com/Caspec/thetrainproject"
              target="_blank"
              >Train project Github code</b-dropdown-item
            >
            <b-dropdown-item
              href="https://github.com/Caspec/mentorwebshop"
              target="_blank"
              >Mentor project Github code</b-dropdown-item
            >
            <b-dropdown-item
              href="https://github.com/Caspec/CPHB-2Semester/tree/master/Fog"
              target="_blank"
              >Fog project Github code</b-dropdown-item
            >
          </b-nav-item-dropdown>
          <b-nav-item href="./cv-casperENG.pdf" target="_blank">CV</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-button class="inTouch" variant="primary" :to="{ name: 'Contact' }"
            >Get In Touch</b-button
          >

          <b-nav-item-dropdown right>
            <template v-slot:button-content>
              <span>Login</span>
            </template>
            <b-dropdown-item href="#">Login</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right>
            <template v-slot:button-content>
              <span
                ><img
                  class="img-fluid"
                  :src="require('../assets/united-kingdom-flag-icon-16.png')"
                  alt="ENG"
                  title="ENG"
                />
                ENG</span
              >
            </template>
            <b-dropdown-item :to="{ name: 'Home' }"
              ><img
                class="img-fluid"
                :src="require('../assets/denmark-flag-icon-16.png')"
                alt="DK"
                title="DK"
              />
              DK</b-dropdown-item
            >
            <b-dropdown-item :to="{ name: 'Home' }"
              ><img
                class="img-fluid"
                :src="require('../assets/united-kingdom-flag-icon-16.png')"
                alt="ENG"
                title="ENG"
              />
              ENG</b-dropdown-item
            >
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {};
</script>

<style>
.navbg {
  background-color: #000;
  padding: 10px;
}

.logotext {
  font-family: "Righteous", cursive;
  text-decoration: none;
  color: #fff;
  font-size: 1.8em;
}

.logotext:hover {
  text-decoration: none;
  color: #2c8fd1;
}

.dropdown-menu {
  background-color: rgb(0, 0, 0) !important;
  color: #fff !important;
}

.dropdown-item {
  background-color: rgb(0, 0, 0) !important;
  color: #c4c4c4 !important;
  font-family: "Roboto", sans-serif;
}

.dropdown-item:hover {
  background-color: rgba(48, 48, 48, 0.79) !important;
  color: #2376ad !important;
  text-decoration: none !important;
}

.nav-link {
  color: #31a0eb !important;
  font-family: "Roboto", sans-serif;
}

.nav-link:hover {
  color: #2c8fd1 !important;
  text-decoration: none !important;
}

.navbar-dark .navbar-toggler {
  border-color: #000 !important;
  color: #000 !important;
  padding-top: 0.6em;
}

.navbar-dark .navbar-toggler-icon {
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' width='30' height='30' viewBox='0 0 30 30'%3e%3cpath stroke='rgba(255, 255, 255)' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e") !important;
}

.inTouch {
  margin-right: 10px !important;
}

@media screen and (max-width: 992px) {
  .nav-space {
    padding-left: 0em;
    margin-left: 0em;
  }
  .dropdown-menu {
    padding-top: 0px !important;
  }
}

@media screen and (min-width: 992px) {
  .nav-space {
    margin-left: 6em;
  }
  .dropdown-menu {
    padding-top: 26px !important;
  }
}
</style>