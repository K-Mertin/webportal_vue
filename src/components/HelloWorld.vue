<template>
  <div class="hello welcome">
    <h1>{{ msg }}</h1>
    <h2>請選擇服務</h2>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.welcome {
   margin-top: 20px;
   color: white;
   font-family:PingFangTC-Regular ;
}
</style>
