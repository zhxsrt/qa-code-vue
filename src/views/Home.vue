<template>
  <div class="home">
    <header-search></header-search>
    <slider class="slider"></slider>
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Slider from '@/components/Slider.vue'
import HeaderSearch from '@/components/HeaderSearch.vue'
export default {
  name: 'home',
  components: {
    HelloWorld,
    Slider,
    HeaderSearch
  }
}
</script>
<style>
.home {
  position: absolute;
  overflow: auto;
  top: 0;
  bottom: 64px;
  right: 0;
  left: 0;
}
.slider {
  margin-top: 48px;
}
</style>
