<template>
  <div>
    <div class="feed">
      <div class="first">
        <Post></Post>
        <Post></Post>
        <Post></Post>
      </div>
      <div class="second">
        <Post></Post>
        <Post></Post>
        <Post></Post>
      </div>
    </div>

    <PostExtended></PostExtended>
  </div>
</template>

<script>
import Post from "@/components/Post.vue";
import PostExtended from "@/components/PostExtended.vue";

export default {
  name: "FeedSection",
  components: {
    Post,
    PostExtended
    // ForgotPassword
  }
};
</script>

<style lang="scss" scoped>
.feed {
  width: 76vw;
  margin: 4.5vw;
  display: flex;
}
.first {
  width: 50%;
  margin-left: 2em;
  margin-right: 0.5em;
}
.second {
  width: 50%;
  margin-right: 2em;
  margin-left: 0.5em;
}
</style>
