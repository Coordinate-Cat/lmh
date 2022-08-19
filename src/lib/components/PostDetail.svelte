<script lang="ts">
  export let post: Post;
  import { format } from "fecha";
</script>

<div class="post-detail__top">
  <h1 class="post-detail__top__title">{post.title}</h1>
  <p>{post.tags}</p>
  <p>{post.description}</p>
  <div class="post-detail__top__info">
    <p class="post-detail__top__info__date">
      {format(new Date(post.date), "MMMM DD, YYYY")},
      <a class="post-detail__top__info__author" href="/about">by Ocat</a>
    </p>
  </div>
</div>

<div class="post-detail">
  <div class="post-detail__content">
    {@html post.body}
  </div>
</div>

<style>
  .post-detail {
    padding: 1rem;
    padding-top: 0;
    /* margin-top: 1rem; */
  }
  .post-detail__top {
    border-bottom: solid 1px var(--border-color);
    padding: 1rem;
    /* margin-bottom: 2rem; */
  }
  .post-detail__top__title {
    margin: 0;
  }
  .post-detail__top__info {
    display: flex;
    flex-direction: row;
  }
  .post-detail__top__info__date {
    color: var(--secondary-color);
  }
  .post-detail__top__info__author {
    margin-left: 0.4rem;
  }
</style>
