<template>
  <default-layout></default-layout>
</template>

<script>
import DefaultLayout from './views/layouts/DefaultLayout'
export default {
  components:{
    DefaultLayout
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  min-height: 100%;
}
</style>
