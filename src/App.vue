<template>
  <div id="nav">
    <button @click="toast">test</button>
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
  },
  methods: {
    toast() {
      this.$toast.show('qqq', 2000);
    }
  }
}

</script>

<style lang="scss">
  //这里使用了别名配置，详情看 vue.config.js
  @import "assets/css/base.css";
</style>
