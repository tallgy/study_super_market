<template>
  <div id="nav">
    <router-view></router-view>
    <main-tab-bar></main-tab-bar>
  </div>
</template>

<script>
import main_tab_bar from './components/content/mainTabBar/mainTabBar';

export default {
  name: 'nav',
  components: {
    main_tab_bar
  }
}

</script>

<style lang="scss">
  //这里使用了别名配置，详情看 vue.config.js
  @import "assets/css/base.css";
</style>
