<template>
  <div class="container">
    <h1>Hello World!</h1>
    <img
      src="/static/logo.png"
      class="logo"
    >
    <input type="text">
    <hr>
    <Counter title="Title from prop" />
  </div>
</template>

<script>
import Counter from './Counter.vue'

export default {
  components: {
    Counter
  }
}
</script>

<style lang="scss" scoped>
  $h1-color: #0a0;

  .container {
    margin: 0 auto;
    max-width: 600px;
    background: url(./assets/logo.svg);
  }
  h1 {
    color: $h1-color;
  }
  .logo {
    display: block;
    width: 100px;
  }
</style>
