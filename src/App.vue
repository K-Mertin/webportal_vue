<template>
  <div id="app" class="multi_bg">
    <!-- <nav  id="nav" class="navbar navbar-expand-lg nav-bg">
      <div class="row">
        <div class="col">
          <a class="navbar-brand" href="#"><img src="./assets/logo.svg" class="logo"></a>
        </div>
        <div class="nav-pipe "></div>        
        <div class="col slogon">
          <div>區塊鏈防偽平台 </div>
          <div>Blockchain Platform </div>
        </div>
      </div>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">About</router-link>
          </li>
        </ul>
      </div>
    </nav> -->
    <Navigation> </Navigation>
    <router-view/>

  </div>
</template>

<script>
// @ is an alias to /src
import Navigation from "./components/Navigation.vue";

export default {
  name: "app",
  components: {
    Navigation
      }
};
</script>

<style>

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  overflow: auto;
}

.back {
  background: #b6d232
}
@media (max-width: 600px) {
  .multi_bg {
    height: -webkit-fill-available;
    background:  #b6d232;
    
    background-image   : url("./assets/bg-1.svg"),
                        url("./assets/bg-2.svg");

    background-repeat  : no-repeat,
                        no-repeat;

    background-position: bottom left,
                        right;

    background-size: auto,
                    auto;

  }
}
@media (min-width: 601px) {
  .multi_bg {
    height: -webkit-fill-available;
    background:  #b6d232;
    
    background-image   : url("./assets/bg-1.svg"),
                        url("./assets/bg-2.svg");

    background-repeat  : no-repeat,
                        no-repeat;

    background-position: bottom left,
                        right;

    background-size: auto,
                    contain;

  }
}

</style>
