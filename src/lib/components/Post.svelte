<script lang="ts">
  export let post: Post;
  import { format } from "fecha";
</script>

<div class="post-item">
  <a class="post-item__title__link" href={`/blog/${post.slug}`}>
    <div class="post-item-left">{post.emoji}</div>
    <div class="post-item-right">
      <h2 class="post-item__title">
          {post.title}
      </h2>
      <!-- <p class="post-item__description">{post.description}</p> -->
      <p class="post-item__date">{format(new Date(post.date), "MMMM DD, YYYY")}</p>
    </div>
  </a>
</div>

<style>
  .post-item {
    border-bottom: solid 1px var(--border-color);
    padding: 0 16px 0 0;
    line-height: 1.6;
  }
  .post-item:last-child {
    border-bottom: none;
  }
  .post-item-left {
    height: fit-content;
    margin: auto 4px;
    font-size: 1.5rem;
  }
  .post-item-right {
    border-left: 1px solid #000;
    padding-left: 4px;
  }
  .post-item__date {
    color: var(--secondary-color);
  }
  .post-item__title {
    line-height: 24px;
    font-size: 1.2rem;
  }
  .post-item__title__link {
    color: var(--main-color);
    font-size: 1.2rem;
    text-decoration: none;
    display: flex;
  }
</style>
