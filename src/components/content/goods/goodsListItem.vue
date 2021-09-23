<template>
  <div @click="imageLoad">
    123
  </div>
</template>

<script>
export default {
  name: "goodsListItem",
  methods: {
    imageLoad() {
      this.$bus.$emit('itemImageLoad');
    }
  }
}
</script>

<style scoped>

</style>
