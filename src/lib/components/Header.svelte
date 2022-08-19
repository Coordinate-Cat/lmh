<script>
  import { blogMetaData } from "$lib/blogMetaData";
</script>

<nav class="header">
  <a href="/" class="header__title">{blogMetaData.blogTitle}</a>
  <ul class="header__links">
    <li class="header__links_item">
      <a href="/" class="header__links__item__link">Home</a>
    </li>
    <li class="header__links_item">
      <a href="/about" class="header__links__item__link">About</a>
    </li>
  </ul>
</nav>

<style>
  .header {
    display: flex;
    /* position: fixed; */
    flex-direction: row;
    justify-content: space-between;

    max-width: calc(100% - 8px);
    margin: 0 auto;
    width: 100%;
    height: 4rem;
    margin: 4px;
    /* margin-top: 4px; */
    margin-bottom: none;

    border: 1px solid #000;
    border-top: none;
  }

  .header__title {
    display: flex;
    flex-direction: row;
    align-items: center;

    padding-right: 16px;
    padding-left: 16px;
    border-right: 1px solid #000;

    color: var(--main-color);
    text-decoration: none;
    font-weight: bold;
    font-size: 1.5rem;
    line-height: 6.2rem;
  }

  .header__links {
    display: flex;
    flex-direction: row;
    align-items: center;
    list-style: none;
  }

  .header__links_item {
    margin-left: 1rem;
  }

  .header__links_item:last-child {
    margin-right: 1rem;
  }

  .header__links__item__link {
    padding-bottom: 0.2rem;
    color: var(--secondary-color);
    text-decoration: none;
  }

  .header__links__item__link:hover {
    border-bottom: 1.5px solid var(--secondary-color);
  }
</style>
