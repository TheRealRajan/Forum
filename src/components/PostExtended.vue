<template>
  <div>
    <div class="post-extended">
      <Post></Post>
      <div class="add-comment">
        <img src="@/assets/profile-img.png" alt />
        <textarea name id cols="85" rows="10" placeholder="Add a comment..."></textarea>
      </div>
      <div class="replies">
        <div class="parent-reply"></div>
        <div class="child-reply"></div>
      </div>
    </div>
  </div>
</template>

<script>
import Post from "@/components/Post.vue";

export default {
  name: "PostExtended",
  components: {
    Post
  }
};
</script>

<style lang="scss" scoped>
.post-extended {
  width: 45%;
  margin: 0 0 0 19.5vw;
}

.add-comment {
  display: flex;
  background: $almostWhite2;
  align-items: flex-start;
  img {
    width: 1.5em;
    margin: 1.5em 1em 1em 1em;
    align-self: flex-start;
  }
  textarea {
    flex-grow: 1;
    background: $white;
    height: 8em;
    margin: 1.5em 1.5em 1.5em 0;
    max-height: 20em;
    padding: 1em;
    border: none;
    border-radius: 5px;
  }
}
</style>
