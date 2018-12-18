<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
  import home from "./components/home/home"
export default {
  name: 'App',
  components:{
    home,
  }
}
</script>

<style>
*{margin:0;padding:0;}
li{list-style:none;}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
body,html{
  font-size: 100px;
  background:#ebebeb;
}
.cf:after{
  content:"";
  display:block;
  clear:both;
}
a{text-decoration: none;}
</style>
