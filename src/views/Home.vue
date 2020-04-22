<template>
  <div>
    <div class="home">
      <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
      <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->

      <SideBar></SideBar>
      <div class="home-container">
        <TopBar></TopBar>
        <ProfileBar></ProfileBar>
        <PostExtended></PostExtended>
        <FeedSection></FeedSection>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import SideBar from "@/components/SideBar.vue";
import TopBar from "@/components/TopBar.vue";
import ProfileBar from "@/components/ProfileBar.vue";
import FeedSection from "@/components/FeedSection.vue";
import PostExtended from "@/components/PostExtended.vue";

export default {
  name: "Home",
  components: {
    SideBar,
    TopBar,
    ProfileBar,
    FeedSection,
    PostExtended
  }
};
</script>

<style lang="scss" scoped>
.home {
  background-color: $almostWhite;
  box-sizing: border-box;
  // height: 100vh;
  // width: 95.5vw;
  // margin: 2em;
}
</style>
