<template>
  <headerTop/>
  <MenuTop/>
  <router-view/>
  <footerTop/>
</template>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1d75ce;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #ca1f1f;
}

nav a.router-link-exact-active {
  color: #062a1a;
}
</style>


<script>
import MenuTop from "@/components/templates/MenuTop";
import headerTop from "@/components/templates/headerTop";
import footerTop from "@/components/templates/footerTop";
export default{
  components:{
    MenuTop,
    headerTop,
    footerTop
  }
}
</script>