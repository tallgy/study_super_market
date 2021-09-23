<template>
  <div id="main_tab_bar">
    <tab-bar>
      <tab-bar-item path="/home">
        <template #item-icon>
          <img src="~assets/img/tabBar/home.png" alt="">
        </template>
        <template #item-icon-active>
          <img src="~assets/img/tabBar/home-active.png" alt="">
        </template>
        <template #item-text>
          <div>首页</div>
        </template>
      </tab-bar-item>

      <tab-bar-item path="/category">
        <template #item-icon>
          <img src="~assets/img/tabBar/category.png" alt="">
        </template>
        <template #item-icon-active>
          <img src="~assets/img/tabBar/category-active.png" alt="">
        </template>
        <template #item-text>
          <div>分类</div>
        </template>
      </tab-bar-item>

      <tab-bar-item path="/cart">
        <template #item-icon>
          <img src="~assets/img/tabBar/cart.png" alt="">
        </template>
        <template #item-icon-active>
          <img src="~assets/img/tabBar/cart-active.png" alt="">
        </template>
        <template #item-text>
          <div>购物车</div>
        </template>
      </tab-bar-item>

      <tab-bar-item path="/profile">
        <template #item-icon>
          <img src="~assets/img/tabBar/profile.png" alt="">
        </template>
        <template #item-icon-active>
          <img src="~assets/img/tabBar/profile-active.png" alt="">
        </template>
        <template #item-text>
          <div>我的</div>
        </template>
      </tab-bar-item>
    </tab-bar>
  </div>
</template>

<script>
import tabBar from 'components/common/tabBar/tabBar';
import tabBarItem from 'components/common/tabBar/tabBarItem'

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
