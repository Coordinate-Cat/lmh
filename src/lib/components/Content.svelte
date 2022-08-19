<div class="content"><slot /></div>

<style>
  .content {
    /* max-width: 760px; */
    /* padding: 1rem; */
    margin: 4px;
    border: 1px solid #000;
    /* margin-top: 72px; */
    /* margin-bottom: 72px; */
    overflow: scroll;
    height: 89vh;
  }
  /*スマホサイズに適用*/
  @media screen and (max-width:599px){
    .content {
      /* max-width: 760px; */
      /* padding: 1rem; */
      margin: 4px;
      border: 1px solid #000;
      /* margin-top: 72px; */
      /* margin-bottom: 72px; */
      overflow: scroll;
      height: 86vh;
    }
  }
</style>
