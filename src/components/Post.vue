<template>
  <div>
    <div class="post-body">
      <div class="vote">
        <button>&#8593;</button>
        <span>69</span>
        <button>&#8595;</button>
      </div>
      <div class="content">
        <span class="title">
          Lorem ipsum, dolor sit amet conturetsti alpidi adipisi elit piliti
          siliti tit.
        </span>
        <span class="flair">Flair</span>
        <div class="description">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Explicabo,
          ex corrupti sapiente accusamus provident nam maiores quibusdam sed
          esse eaque inventore, quos impedit adipisci eius dolorum eveniet
          distinctio et unde?
        </div>

        <div class="divider"></div>
        <div class="metadata">
          <div class="post-details">
            <img style="width:1.1em; height:1.1em;" src="@/assets/profile-img.png" alt />
            <div class="username">
              <span class="posted">Posted By:</span>
              <span class="name">Prakash Badal</span>
            </div>
            <div class="post-time">2 hrs ago</div>
          </div>
          <div class="comment-count">
            <svg class="svg-img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
              <path
                d="M448 0H64C28.7 0 0 28.7 0 64v288c0 35.3 28.7 64 64 64h96v84c0 7.1 5.8 12 12 12 2.4 0 4.9-.7 7.1-2.4L304 416h144c35.3 0 64-28.7 64-64V64c0-35.3-28.7-64-64-64zm16 352c0 8.8-7.2 16-16 16H288l-12.8 9.6L208 428v-60H64c-8.8 0-16-7.2-16-16V64c0-8.8 7.2-16 16-16h384c8.8 0 16 7.2 16 16v288z"
              />
            </svg>
            <span>100 +</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Post"
};
</script>

<style lang="scss" scoped>
.post-body {
  display: flex;
  flex-direction: row;
  padding: 1.5em 2em 1.5em 0;
  background: #ffffff;
  border-radius: 5px;
  margin: 0 0 1em;
}
.vote {
  display: flex;
  font-size: 0.9em;
  flex-direction: column;
  align-items: center;
  padding: 0 1em 1em 1em;

  button,
  span {
    font-size: 1.1em;
    line-height: 1;
    padding-bottom: 0.5em;
    border: none;
    background: none;
  }
}

.title {
  font-weight: bold;
}
.description {
  font-size: 0.8em;
  margin-top: 0.5em;
  color: $lightText;
  word-spacing: 0.1em;
}

.divider {
  background: $almostWhite;
  height: 2px;
  margin: 1em 0;
}

.metadata {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  font-size: 0.8em;
}
.post-details {
  width: 80%;
  display: flex;
  align-items: center;

  .post-time {
    color: $lightText2;
  }

  .username {
    margin: 0 2em 0 1em;
    .posted {
      color: $lightText2;
    }
    .name {
      color: $primaryBlue;
    }
  }
}
.comment-count {
  //   width: 20%;
  color: $lightText2;

  .svg-img {
    width: 0.8em;
    fill: #aaaaaa;
  }
}

.flair {
  background: $primaryBlue;
  margin-left: 1em;
  text-transform: uppercase;
  text-align: center;
  font-size: 0.7em;
  color: #fff;
  padding: 0 0.8em;
  border-radius: 3px;
  line-height: 1;
}
</style>
