<template>
  <div>
    <div id="container">
    <div id="contacts">
      <div id="contacts--social" class="mt-2">
        <div class="mt-1">
        <a href="https://github.com/Caspec" target="_blank"> 
            <img class="img-fluid" :src="require('../assets/GitHub_Logo_White.png')" alt="Social" />
        </a>
        </div>
        <div class="ml-2">
        <a href="https://www.linkedin.com/pub/casper-christensen/22/70b/8a4" target="_blank"> 
            <img class="img-fluid" :src="require('../assets/LI-In-Bug.png')" alt="Social" />
        </a>
        </div>
        <div class="ml-2 mt-1">
        <a href="https://twitter.com/followcasper88" target="_blank"> 
            <img class="img-fluid" :src="require('../assets/Twitter_Social_Icon_Circle_Color.png')" alt="Social" />
        </a>
        </div>
      </div>
    </div>
    <div id="mentions" class="mt-4 pt-4">
      <p>&copy; 2020 Casper - Full Stack Web developer </p>
    </div>
   </div>
  </div>
</template>

<script>
export default {

};
</script>

<style>

#container{
  padding-top: 20px;
  margin-top: 20px;
  /*width:100vw;*/
  color:white;
  background-color:#151515;
  display: flex;
  flex-direction: column;
  align-items: center;
}
#contacts{
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 100%;
}
#contacts--social{
  width: 15%;
  display : flex;
  justify-content : space-between;
}

@media screen and (max-width: 768px) {
 #contacts--social { 
  width: 40%;
 }
}

@media screen and (max-width: 1200px) {
 #contacts--social { 
  width: 30%;
 }
}

#mentions p {
  font-size: 1em;
  font-family: "Open Sans", sans-serif;
}

</style>