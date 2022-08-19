<footer class="footer">
  <ul class="footer__links">
    <li class="footer__links_item">
      <a href="/" class="footer__links__item__link">Home</a>
    </li>
    <li class="footer__links_item">
      <a href="/about" class="footer__links__item__link">About</a>
    </li>
    <li class="footer__links_item">
      <a href="/rss.xml" class="footer__links__item__link">RSS Feed</a>
    </li>
    <li class="footer__links_item">
      <span class="footer__copy-right">© 2021 Ocat</span>
    </li>
  </ul>
</footer>

<style>
  .footer {
    /* position: fixed; */
    border: 1px solid #000;
    margin: 4px;
    bottom: 0;
    /* height: 2rem; */
    display: flex;
    flex-direction: row;
  }

  .footer__links {
    display: flex;
    /* flex-direction: row;
    align-items: center; */
    list-style: none;
  }

  ul.footer__links {
    margin: 0 16px;
  }

  .footer__links_item {
    margin: 0;
  }
  /* 最初の要素以外 */
  .footer__links_item:not(:first-child) {
    margin-left: 1rem;
  }

  .footer__links_item:last-child {
    margin-right: 1rem;
  }

  .footer__links__item__link {
    padding-bottom: 0.2rem;
    color: var(--secondary-color);
    text-decoration: none;
  }

  .footer__links__item__link:hover {
    border-bottom: 1.5px solid var(--secondary-color);
  }

  .footer__copy-right {
    color: var(--secondary-color);
  }
</style>
