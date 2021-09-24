<template>
  <div class="toast" v-show="show">
    <div>{{message}}</div>
  </div>
</template>

<script>
export default {
  name: "toast",
  props: {
    message: {
      type: String,
      default: ''
    },
    show: {
      type: Boolean,
      default: false
    }
  },
  data() {
    return {
      message: '',
      show: false
    };
  },
  methods: {
    show(message, duration) {
      this.show = true;
      this.message = message;

      setTimeout(() => {
        this.show = false;
        this.message = '';
      }, duration);

    }
  }
}
</script>

<style scoped>

</style>
