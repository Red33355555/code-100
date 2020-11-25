<template>
  <footer>
      <slot></slot>
  </footer>
</template>

<script>
export default {
    name:'footer-component'
}
</script>

<style lang="scss" scoped>
footer {
  position: fixed;
  bottom: 0;
  background-color: blue;
  color: white;
  height: 10vh;
  width: 100%;
}
</style>