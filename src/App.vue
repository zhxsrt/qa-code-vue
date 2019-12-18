<template>
  <div id="app">
    <router-view class="router-view-content"/>
    <bottom-nav></bottom-nav>
  </div>
</template>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100vh;
  position: relative;
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
.router-view-content{
  bottom: 64px;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  overflow: auto;
}
/* .router-view-content:after{
  content: "";
  display: block;
  clear: both;
} */
</style>
<script>
import BottomNav from './components/BottomNav.vue'
export default {
  components: { BottomNav }
}
</script>
