<template>
  <div id="home">
    <nav-bar class="home-nav"><template #center>购物街</template></nav-bar>
    <home-swiper :banners="banners"></home-swiper>
    <goods-list-item></goods-list-item>
  </div>
</template>

<script>
import navBar from 'components/common/navBar/navBar'
import goodsListItem from 'components/content/goods/goodsListItem'

import homeSwiper from './childComps/homeSwiper'

import { getHomeMul, getHomeGoods } from 'network/home'

export default {
  name: "home",
  components: {
    navBar,
    homeSwiper,
    goodsListItem
  },
  data() {
    return {
      banners: [],
      recommends: []
    }
  },
  created() {
    getHomeMul().then(res => {
      console.log(res);
      this.banners = res.data.banners;
      this.recommends = res.data.recommends;
    }, err => {
      console.log(err);
    })

    this.$bus.$on('itemImageLoad', () => {
      console.log('----');
    })
  }
}
</script>

<style scoped>
.home-nav {
  background-color: var(--color-tint);
  color: #fff;
}
</style>
