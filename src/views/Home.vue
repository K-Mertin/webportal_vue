<template>
  <div class="container">
    <div class="home">
      <HelloWorld msg="歡迎您!XXXXXX"/>
    </div>
    <div class="row service-contain">
      <div class="col-md-6 col-lg-4 col-sm-6 col-xs-6 col-6">
        <div class="service-block">
          <div class="service-icon">
            <img src="../assets/contract.svg">
            <img src="../assets/contract_hover.svg" class="img-top">
            <div class="row">
                123123132
            </div>
            
          </div>
        </div>
      </div>
      <div class="col-md-6 col-lg-4 col-sm-6 col-xs-6 col-6">
        <div class="service-block"></div>
      </div>
      <div class="col-md-6 col-lg-4 col-sm-6 col-xs-6 col-6">
        <div class="service-block"></div>
      </div>
      <div class="col-md-6 col-lg-4 col-sm-6 col-xs-6 col-6">
        <div class="service-block"></div>
      </div>
      <div class="col-md-6 col-lg-4 col-sm-6 col-xs-6 col-6">
        <div class="service-block"></div>
      </div>
      <div class="col-md-6 col-lg-4 col-sm-6 col-xs-6 col-6">
        <div class="service-block"></div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "home",
  components: {
    HelloWorld
  }
};
</script>


<style scoped>
.service-icon {
  position: relative;
  display: inline-block;
  border: 1px;
  border-color:black;
  border-style: solid;
  margin: 20px;
}
.service-icon .img-top {
  display: none;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 99;
}
.service-icon:hover .img-top {
  display: inline;
}
.service-contain {
  padding: 5px;
  overflow: auto;
}
.service-block {
  width: 140px;
  height: 182px;
  border-radius: 10px;
  box-shadow: 0 5px 10px 0 rgba(0, 0, 0, 0.1);
  background-color: var(--white);
  margin: 5px;
}
@media screen and (min-width: 576px) {
  .service-block {
    width: 250px;
    height: 182px;
    border-radius: 10px;
    box-shadow: 0 5px 10px 0 rgba(0, 0, 0, 0.1);
    background-color: var(--white);
    margin: 10px;
  }
}
@media screen and (min-width: 768px) {
  .service-block {
    width: 300px;
    height: 182px;
    border-radius: 10px;
    box-shadow: 0 5px 10px 0 rgba(0, 0, 0, 0.1);
    background-color: var(--white);
    margin: 10px;
  }
}
@media screen and (min-width: 992px) {
  .service-block {
    width: 350px;
    height: 182px;
    border-radius: 10px;
    box-shadow: 0 5px 10px 0 rgba(0, 0, 0, 0.1);
    background-color: var(--white);
    margin: 10px;
  }
}
</style>
