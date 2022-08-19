<script lang="ts">
  export let post: Post;
  import { format } from "fecha";
</script>

<div class="post-item">
  <h2 class="post-item__title">
    <a class="post-item__title__link" href={`/blog/${post.slug}`}
      >{post.title}</a
    >
  </h2>
  <!-- <p class="post-item__description">{post.description}</p> -->
  <p class="post-item__date">{format(new Date(post.date), "MMMM DD, YYYY")}</p>
</div>

<style>
  .post-item {
    border-bottom: solid 1px var(--border-color);
    padding: 0 16px;
    line-height: 1.6;
  }
  .post-item:last-child {
    border-bottom: none;
  }
  .post-item__date {
    color: var(--secondary-color);
  }
  .post-item__title {
    line-height: 24px;
  }
  .post-item__title__link {
    color: var(--main-color);
    font-size: 1.2rem;
    text-decoration: none;
  }
</style>
