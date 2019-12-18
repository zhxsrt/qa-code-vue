<template>
  <nav class="bottom-nav">
    <router-link to="/">
      <i></i>
      <span>首页</span>
    </router-link>
    <router-link to="/lib">
      <i></i>
      <span>题库</span>
    </router-link>
    <router-link to="/connect">
      <i></i>
      <span>交流</span>
    </router-link>
    <router-link to="/user">
      <i></i>
      <span>我的</span>
    </router-link>
  </nav>
</template>

<script>
export default {}
</script>

<style>
.bottom-nav{
  display: flex;
  height: 64px;
  justify-content: space-evenly;
  background: #ddd;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
}
.bottom-nav a{
  flex-grow: 1;
  align-items: center;
  /* line-height: 64px; */
  text-decoration: none;
  color: #888;
  display: flex;
  flex-direction: column;
  justify-content: center;
  font-size: 10px;
}
.bottom-nav a i{
  height: 32px;
  width: 32px;
  background: #fdfdfd;
}
</style>
