<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link>|
      <router-link to="/about">About</router-link>
    </div>-->
    <!-- <router-view /> -->
    <Home></Home>
    <!-- <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Natus, quaerat.</p> -->
  </div>
</template>

<script>
import Home from "@/views/Home";

export default {
  components: {
    Home
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Manrope:wght@400;600&display=swap");

// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
// }

// #nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
body {
  font-family: "Manrope";
  margin: 0;
}
.test {
  background: $warning;
  font-size: 3rem;
}
</style>
