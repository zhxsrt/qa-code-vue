<template>
  <header>
    <form @submit.prevent>
      <div class="search-input-wrap">
        <input v-model="searchValue" />
        <i class="search btn"></i>
      </div>
      <div class="search-input-right-btn">
        <i v-if="isSearch">信息</i>
        <button
          v-else
          @click="rollback"
        >取消</button>
      </div>
    </form>
  </header>
</template>

<script>
export default {
  data () {
    return {
      isSearch: true,
      searchValue: ''
    }
  }
}
</script>

<style>
header {
  height: 48px;
  background: #42b983;
  z-index: 1000;
  position: fixed;
  top: 0;
  width: 100vw;
}
header form {
  position: relative;
  height: 100%;
}
header form .search-input-wrap {
  position: absolute;
  height: 100%;
  right: 56px;
  left: 0;
  line-height: 48px;
}
header form .search-input-right-btn {
  position: absolute;
  right: 0;
  height: 100%;
  line-height: 48px;
  width: 56px;
  text-decoration: none;
}
header form .search-input-right-btn i,
header form .search-input-right-btn button {
  font-style: normal;
  color: #fff;
}
header form .search-input-wrap input {
  height: 28px;
  width: 90%;
  border-radius: 28px;
  border: none;
}
header form .search-input-wrap input:focus {
  outline: none;
}
</style>
