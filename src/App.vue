<template>
  <div id="app">
    <router-view></router-view>
    <main-tab-bar/>
  </div>
</template>

<script>
import MainTabBar from './components/content/mainTabbar/MainTabBar.vue'
import router from './router/index'
export default {
  name: 'app',
  components: {
    MainTabBar
  },
  router
}
</script>

<style>
  @import "./assets/css/base.css";
</style>
