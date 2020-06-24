<template>
  <div>
    <div class="home">
      <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
      <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->

      <TopBar></TopBar>
      <SideBar></SideBar>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import SideBar from "@/components/Sidebar.vue";
import TopBar from "@/components/TopBar.vue";

export default {
  name: "Home",
  components: {
    SideBar,
    TopBar
    // HelloWorld
  }
};
</script>

<style lang="scss" scoped>
.home {
  background-color: $almostWhite;
  box-sizing: border-box;
  height: 100vh;
  // width: 95.5vw;
  // margin: 2em;
}
</style>
