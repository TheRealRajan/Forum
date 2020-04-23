<template>
  <div>
    <div class="post-extended">
      <!-- <Post></Post> -->
      <div class="post-body">
        <div class="vote">
          <button>&#8593;</button>
          <span>69</span>
          <button>&#8595;</button>
        </div>
        <div class="content">
          <span class="title">
            Lorem ipsum, dolor sit amet conturetsti alpidi adipisi elit piliti
            siliti tit pirit chilit lilit.
          </span>
          <span class="flair">Flair</span>
          <div class="description">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae
            mollitia vero pariatur accusantium nam, ut porro corporis eius!
            Tempora, omnis nihil rerum modi quaerat earum officia illo
            perspiciatis amet eius possimus animi architecto enim repudiandae
            aspernatur est cupiditate cum corrupti magni officiis impedit odio.
            Perspiciatis minus placeat eos obcaecati rerum.
          </div>
        </div>
      </div>

      <section class="lower-section">
        <div class="add-comment">
          <img src="@/assets/profile-img.png" alt />
          <textarea placeholder="Add a comment..."></textarea>
        </div>
        <div class="replies-section">
          <div class="wrapper">
            <div class="vote">
              <img style="height:1.5em; margin:0.5em 0;" src="@/assets/profile-img.png" alt />
              <button>&#8593;</button>
              <span>69</span>
              <button>&#8595;</button>
            </div>

            <div class="parent-reply">
              <div class="parent-reply-user reply">
                <span class="user parent-user">Piscal Jharel</span>

                <span class="post-time">2 hrs ago</span>
              </div>
              <div class="description">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. In,
                aliquam expedita? Sunt deserunt delectus alias ad iure omnis
                officia eos, fuga itaque voluptates fugit architecto ipsum modi
                distinctio dicta voluptatibus et, reprehenderit, neque
                temporibus totam repudiandae est a facilis! Quos.
              </div>
              <div class="options">
                <span>
                  <button>Reply</button>
                  <button>Share</button>
                  <button>Report</button>
                </span>

                <button>***</button>
              </div>
            </div>
          </div>
          <div class="child-reply">
            <div class="wrapper">
              <div class="vote">
                <img style="height:1.5em; margin:0.5em 0;" src="@/assets/profile-img.png" alt />
                <button>&#8593;</button>
                <span>69</span>
                <button>&#8595;</button>
              </div>

              <div class="parent-reply">
                <div class="parent-reply-user reply">
                  <span class="user parent-user">Prakash Taj Badal</span>

                  <span class="post-time">2 hrs ago</span>
                </div>
                <div class="description">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. In,
                  aliquam expedita? Sunt deserunt delectus alias ad iure omnis
                  officia eos, fuga itaque voluptates fugit architecto ipsum
                  modi distinctio dicta voluptatibus et?
                </div>
                <div class="options">
                  <span>
                    <button>Reply</button>
                    <button>Share</button>
                    <button>Report</button>
                  </span>

                  <button>***</button>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="replies-section">
          <div class="wrapper">
            <div class="vote">
              <img style="height:1.5em; margin:0.5em 0;" src="@/assets/profile-img.png" alt />
              <button>&#8593;</button>
              <span>69</span>
              <button>&#8595;</button>
            </div>

            <div class="parent-reply">
              <div class="parent-reply-user reply">
                <span class="user parent-user">Tikhor Rumal Jhatka</span>

                <span class="post-time">2 hrs ago</span>
              </div>
              <div class="description">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. In,
                aliquam expedita? Sunt deserunt delectus alias ad iure omnis
                officia eos, fuga itaque voluptates fugit architecto ipsum modi
                distinctio dicta voluptatibus et, reprehenderit, neque
                temporibus totam repudiandae est a facilis! Quos.
              </div>
              <div class="options">
                <span>
                  <button>Reply</button>
                  <button>Share</button>
                  <button>Report</button>
                </span>

                <button>***</button>
              </div>
            </div>
          </div>
          <div class="child-reply">
            <div class="wrapper">
              <div class="vote">
                <img style="height:1.5em; margin:0.5em 0;" src="@/assets/profile-img.png" alt />
                <button>&#8593;</button>
                <span>69</span>
                <button>&#8595;</button>
              </div>

              <div class="parent-reply">
                <div class="parent-reply-user reply">
                  <span class="user parent-user">Prakash Taj Badal</span>

                  <span class="post-time">2 hrs ago</span>
                </div>
                <div class="description">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. In,
                  aliquam expedita? Sunt deserunt delectus alias ad iure omnis
                  officia eos, fuga itaque voluptates fugit architecto ipsum
                  modi distinctio dicta voluptatibus et?
                </div>
                <div class="options">
                  <span>
                    <button>Reply</button>
                    <button>Share</button>
                    <button>Report</button>
                  </span>

                  <button>***</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
// import Post from "@/components/Post.vue";

export default {
  name: "PostExtended",
  components: {
    // Post
  }
};
</script>

<style lang="scss" scoped>
.post-extended {
  width: 45%;
  margin: 0 0 0 19.5vw;
  padding-bottom: 1.5rem;
  background: $white;
}

.add-comment {
  display: flex;
  background: $almostWhite2;
  align-items: flex-start;
  // margin-left: 3.5rem;
  img {
    width: 1.5em;
    margin: 1.5em 1em 1em 1em;
    align-self: flex-start;
  }
  textarea {
    font-family: Manrope;
    flex-grow: 1;
    background: $white;
    height: 5rem;
    margin: 1.5em 2em 1.5em 0;
    max-height: 20em;
    padding: 1em;
    border: none;
    border-radius: 5px;
  }
}

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

  button {
    border: none;
    background: none;
    .svg-img {
      width: 0.8em;
      fill: #aaaaaa;
    }
  }

  span {
    font-size: 1.1rem;
    line-height: 1;
    padding: 0.5em 0;
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

// .metadata {
//   display: flex;
//   flex-direction: row;
//   justify-content: space-between;
//   font-size: 0.8em;
// }
.post-details {
  width: 80%;
  display: flex;
  align-items: center;

  // .post-time {
  //   color: $lightText2;
  // }

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

  .comment-num {
    margin-left: 0.25em;
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

.lower-section {
  margin-left: 3.5rem;

  .replies-section {
    margin-top: 1em;
    padding-top: 1em;
    background: $almostWhite2;
    display: flex;
    flex-direction: column;
  }
  .wrapper {
    display: flex;
    background: $almostWhite2;
  }
  .parent-reply {
    display: flex;
    flex-direction: column;
    margin: 0.5em 1.5em 0.5em 0;
  }

  .user {
    color: $primaryBlue;
    font-size: 0.9rem;
  }
  .post-time {
    color: $lightText2;
    font-size: 0.8rem;
  }

  .options {
    display: flex;
    justify-content: space-between;
    margin-top: 0.5em;

    button {
      background: none;
      border: none;
      cursor: pointer;
      color: $lightText2;
      font-size: 0.7rem;
      margin-right: 1em;
    }
  }

  .parent-reply-user {
    // width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    // margin: 0.5em 1em 0.5em 0;
  }

  .child-reply {
    margin-left: 3.5rem;
    margin-top: 1em;
  }
}
</style>
