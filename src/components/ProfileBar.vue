<template>
  <div>
    <div class="user-profile">
      <div class="parent">
        <div class="user">
          <img style src="@/assets/profile-img.png" alt="x" />
          <div>Prakash Raj Badal</div>
        </div>
        <img class="cross" src="@/assets/cross.svg" alt="x" />
      </div>

      <button class="create-button">
        <span>+ Create a Discussion</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProfileBar"
};
</script>

<style lang="scss" scoped>
.user-profile {
  position: sticky;
  height: 100vh;
  background: #fff;
  width: 18vw;
  float: right;
  box-shadow: -1px 0px 15px 2px $cardShadow;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
}

.parent {
  margin: 2em 1em;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.user {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-left: 1.5em;
  font-size: 1em;
  font-weight: 500;
  img {
    width: 5em;
    padding-bottom: 0.5em;
  }
}
.cross {
  width: 0.8em;
  margin: 0 0 5.8em 1em;
}
.create-button {
  width: 80%;
  background: $purple;
  font-size: 0.8em;
  color: #fff;
  border: none;
  border-radius: 5px;
  padding: 0.5em;
  margin-bottom: 2em;
  text-align: center;
  box-shadow: 1px 0px 15px 2px $cardShadow;
  &:hover {
    box-shadow: 1px 1px 5px $purple;
    transition: linear 0.2s;
  }
}
</style>
