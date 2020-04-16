-<template>
  <div>
    <div class="sidebar">
      <!-- <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">
        <path
          d="M328 0h-16a16 16 0 0 0-16 16v480a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V16a16 16 0 0 0-16-16zm-96 96h-16a16 16 0 0 0-16 16v288a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V112a16 16 0 0 0-16-16zm192 32h-16a16 16 0 0 0-16 16v224a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V144a16 16 0 0 0-16-16zm96-64h-16a16 16 0 0 0-16 16v352a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V80a16 16 0 0 0-16-16zM136 192h-16a16 16 0 0 0-16 16v96a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16v-96a16 16 0 0 0-16-16zm-96 32H24a16 16 0 0 0-16 16v32a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16v-32a16 16 0 0 0-16-16zm576 0h-16a16 16 0 0 0-16 16v32a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16v-32a16 16 0 0 0-16-16z"
        />
      </svg>-->
      <img class="icon" src="@/assets/waveform.svg" style="width:2.3em; margin-top:2.5em" />

      <div class="sidebar-contents">
        <!-- <svg
          xmlns="http://www.w3.org/2000/svg"
          width="36.003"
          height="35.339"
          viewBox="0 0 36.003 35.339"
          style="fill:#3953dc"
        >
          <g transform="translate(-0.025)">
            <g transform="translate(0.025 0)">
              <path
                class="a"
                d="M1.537,19.544a1.527,1.527,0,0,1-1.081-2.59L16.946.464A1.533,1.533,0,0,1,18.009,0h0A1.533,1.533,0,0,1,19.09.446l16.49,16.49A1.529,1.529,0,1,1,33.418,19.1L18.009,3.665,2.618,19.111A1.527,1.527,0,0,1,1.537,19.544Z"
                transform="translate(-0.025 0)"
              />
              <path
                class="a"
                d="M28.1,43.151H13.382A6.407,6.407,0,0,1,7,36.744V21.6a1.527,1.527,0,1,1,3.054,0V36.744A3.353,3.353,0,0,0,13.407,40.1H28.126a3.353,3.353,0,0,0,3.3-3.353V21.6a1.527,1.527,0,1,1,3.054,0V36.744A6.407,6.407,0,0,1,28.1,43.151Z"
                transform="translate(-2.74 -7.812)"
              />
              <path
                class="a"
                d="M30.078,41.523H21.527A1.521,1.521,0,0,1,20,40V35.812a5.8,5.8,0,1,1,11.6,0V40a1.521,1.521,0,0,1-1.527,1.527Zm-7.024-3.054h5.5V35.812a2.748,2.748,0,1,0-5.5,0Z"
                transform="translate(-7.8 -11.681)"
              />
            </g>
          </g>
        </svg>-->
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
  name: "SideBar"
};
</script>

<style lang="scss" scoped>
.sidebar {
  height: 100vh;
  width: 4.5vw;
  min-width: 3.5vw;
  background: #fff;
  box-shadow: 1px 0px 15px $cardShadow;
  display: flex;
  flex-direction: column;
  align-items: center;
  position: fixed;

  svg {
    fill: $lightText;
    cursor: pointer;
    width: 7em;
    &:hover,
    &:focus,
    &:active {
      fill: $primaryBlue;
    }
  }
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
