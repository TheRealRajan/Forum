<template>
  <div>
    <div class="topbar">
      <div class="title-text">
        <span class="your">Your &nbsp;</span>
        <span class="feed">Feed</span>
      </div>
      <div class="search-bar">
        <input type="search" placeholder="Search For Topics..." />
        <div class="search-icon">
          <svg
            style="width:1em; height:1em"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 512 512"
          >
            <path
              d="M508.5 468.9L387.1 347.5c-2.3-2.3-5.3-3.5-8.5-3.5h-13.2c31.5-36.5 50.6-84 50.6-136C416 93.1 322.9 0 208 0S0 93.1 0 208s93.1 208 208 208c52 0 99.5-19.1 136-50.6v13.2c0 3.2 1.3 6.2 3.5 8.5l121.4 121.4c4.7 4.7 12.3 4.7 17 0l22.6-22.6c4.7-4.7 4.7-12.3 0-17zM208 368c-88.4 0-160-71.6-160-160S119.6 48 208 48s160 71.6 160 160-71.6 160-160 160z"
            />
          </svg>
        </div>
      </div>

      <div class="sort-by">
        <span>Sort By:</span>
        <select name="sortBy">
          <option value="popular">Popular</option>
          <option value="recent">Recent</option>
          <option value="top">Top</option>
        </select>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TopBar"
};
</script>

<style lang="scss" scoped>
.topbar {
  float: left;
  width: 76vw;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 2em;
  margin-left: 4.5vw;
}

.title-text {
  font-size: 1.5em;
  letter-spacing: 0.05em;
  display: flex;
  flex-direction: row;
  align-items: center;
  color: $darkText;

  .your {
    font-weight: 300;
    margin-right: 0.25em;
  }
  .feed {
    font-weight: 600;
    &::before {
      content: " ";
    }
  }
}

.search-bar {
  font-size: 1em;
  width: 18em;
  max-width: 20em;
  border-radius: 5px;
  border: 1px black;
  display: flex;
  flex-direction: row;
  align-items: center;

  input {
    border: none;
    height: 100%;
    width: 88%;
    padding-left: 1em;
  }
  &::placeholder {
    font-size: 1em;
    color: $lightText2;
  }
  .search-icon {
    width: 12%;
    height: 100%;
    padding: 0.5em;
    background: #fff;

    cursor: pointer;
    svg {
      fill: $lightText2;
    }
  }
}
.sort-by {
  // width: 7.5em;
  font-size: 0.9em;
  line-height: 1;
  padding: 0.5em;
  background: #fff;
  display: flex;
  flex-direction: row;
  align-items: center;
  border-radius: 5px;
  color: $lightText2;

  select {
    border: none;
    font-size: 1em;
    color: $darkText;
    cursor: pointer;
  }
}
</style>
