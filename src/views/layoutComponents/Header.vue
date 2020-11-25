<template>
  <header>
    <slot></slot>
    <slot name="nav"></slot>
  </header>
</template>

<script>
export default {
    name:'header-component'
}
</script>

<style lang="scss" scoped>
header {
  position: fixed;
  background-color: black;
  color: white;
  height: 10vh;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>