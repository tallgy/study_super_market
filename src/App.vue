<template>
  <div id="nav">
    <router-view></router-view>
    <main-tab-bar></main-tab-bar>
  </div>
</template>

<script>
import mainTabBar from 'components/content/mainTabBar/mainTabBar';

export default {
  name: 'nav',
  components: {
    mainTabBar
  }
}

</script>

<style lang="scss">
  //这里使用了别名配置，详情看 vue.config.js
  @import "assets/css/base.css";
</style>
