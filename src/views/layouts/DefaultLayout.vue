<template>
  <header-component>
    <div>
      <!-- <button @click="setOpenSidebar">sidebar</button> -->
      <MenuIcon @click="setOpenSidebar"/>
      <span>Code-100</span>
    </div>
    <template v-slot:nav> </template>
  </header-component>
  <main>
    <side-bar :openSidebar="openSidebar"></side-bar>
  </main>
  <footer-component>This is footer</footer-component>
</template>

<script>
import SideBar from '../layoutComponents/SideBar';
import FooterComponent from '../layoutComponents/Footer';
import HeaderComponent from '../layoutComponents/Header';
import MenuIcon from 'vue-material-design-icons/auto-fix.vue';
export default {
    components:{
        SideBar,
        FooterComponent,
        HeaderComponent,
        MenuIcon
    },
data(){
    return{
      openSidebar:false
    };
  },
  methods:{
      setOpenSidebar(){
          this.openSidebar = !this.openSidebar;
      }
  }
}
</script>

<style lang="scss" scoped>
main {
  background-color: red;
  color: white;
  padding: 10vh 0;
  min-height: 100vh;
  width: 100%;
}
</style>