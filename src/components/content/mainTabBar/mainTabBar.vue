<template>
  <div id="main_tab_bar">
    <router-view></router-view>
    <tab-bar>
      <tab-bar-item path="/home" activeColor="blue">
          <img src="" alt="">
          <img src="active" alt="">
          <div>首页</div>
      </tab-bar-item>
      <tab-bar-item path="/category" activeColor="red">
          <img src="" alt="">
        <img src="active" alt="">
          <div>分类</div>
      </tab-bar-item>
      <tab-bar-item path="/cart" activeColor="blue">
          <img src="" alt="">
        <img src="active" alt="">
          <div>购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile" activeColor="blue">
          <img src="" alt="">
        <img src="active" alt="">
          <div>我的</div>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import tabBar from './components/common/tabBar/tabBar';
import tabBarItem from './components/common/tabBar/tabBarItem'

export default {
  name: "main_tab_bar",
  components: {
    tabBar,
    tabBarItem
  }
}
</script>

<style scoped>

</style>
