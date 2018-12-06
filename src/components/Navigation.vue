<template>
  <nav id="nav" class="navbar navbar-expand-md mb-4 nav-bg">
      <a class="navbar-brand" href="#">
        <img src="../assets/logo.svg" class="logo">
      </a>
      <hr class="nav-pipe"><div class="slogon mr-auto">
        <div>區塊鏈防偽平台</div>
        <div>Blockchain Platform</div>
      </div>

      <div class="navbar-nav flex-row ml-md-auto d-none d-md-flex">
          <a
            class="nav-link dropdown-toggle"
            href="#"
            id="navbarDropdown"
            role="button"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >繁體中文</a>
          <div id="language-menu" class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item" href="#">繁體中文</a>
          </div>
          <div class="col-1"> 
            <div :class="{'oval':loggin, 'oval_out':!loggin}">
              <img src="../assets/smile.svg" v-on:click="loginout">
            </div>
            
          </div>      
      </div>
    
    <!-- <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">About</router-link>
          </li>
        </ul>
    </div>-->
  </nav>
 
</template>

<script>
export default {
  name: "Navigation",
  props: {
    msg: String
  },
  data() {
    return {
      loggin: false
    }
  },
  methods:{
    loginout: function () {
      this.loggin = !this.loggin;
    }
  }
};
</script>

<style>
.status {
  float: right;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.nav-bg {
  width: 100%;
  height: 70px;
  box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.1);
  background-color: var(--white);
}
.logo {
  width: 140px;
  height: 30px;
  object-fit: contain;
}
.nav-pipe {
  width: 1px;
  height: 30px;
  margin-left: 0px;
  margin-right: 10px;
  background-color: #dddddd;
}
.slogon {
  text-align: left;
  font-family: PingFangTC-Regular;
  color: #565454;
}
.oval {
  width: 40px;
  height: 40px;
  border-color: black;
  border: 2px;
  border-style: solid;
  border-radius: 50%;
  padding: 1px;
}
.oval_out {
  width: 40px;
  height: 40px;
  color: transparent;
  border: 2px;
  border-style: solid;
  border-radius: 50%;
  padding: 1px;
}
#language-menu {
  left: auto;
}


</style>
