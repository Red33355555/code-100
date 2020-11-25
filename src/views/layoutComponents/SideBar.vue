<template>
  <div class="sidebar" v-show="openSidebar">
    <ul>
      <li>1</li>
      <li>2</li>
      <li>3</li>
      <li>4</li>
      <li>5</li>
    </ul>
  </div>
</template>

<script>
export default {
    name:'side-bar',
    props:{
        openSidebar:{
            type:Boolean,
            required:true
        }
    }
}
</script>

<style lang="scss" scoped>
.sidebar {
  position: fixed;
  color: black;
  background-color: rgb(131, 209, 144);
  min-height: 80vh;
  top: 10vh;
  bottom: 10vh;
  left: 0;
  width: 250px;
  z-index: 1;
}
</style>