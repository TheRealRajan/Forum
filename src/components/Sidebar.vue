-<template>
  <div>
    <div class="sidebar">
      <img class="icon" src="@/assets/waveform.svg" style="width:2.3em" />

      <div class="sidebar-contents">
        <img class="icon" src="@/assets/home.svg" alt />
        <img class="icon" src="@/assets/compass.svg" alt />
        <img class="icon" src="@/assets/bell.svg" alt />
      </div>
      <img class="icon" src="@/assets/back.svg" alt />
    </div>
  </div>
</template>

<script>
export default {
  name: "Sidebar"
};
</script>

<style lang="scss" scoped>
.sidebar {
  height: 100vh;
  width: 4.5vw;
  background: #fff;
  box-shadow: 1px 0px 15px $cardShadow;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: fixed;
}

.sidebar-contents {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 80%;
  margin: 26vh 0;
}
.icon {
  width: 1.8em;
  max-height: 1.8em;
  margin: 1.2em 0;
  cursor: pointer;

  &:hover,
  &:focus {
    fill: $primaryBlue;
  }
}
</style>
