<div class="content"><slot /></div>

<style>
  .content {
    margin: 4px;
    border: 1px solid #000;
    height: calc(100vh - 76px);
    overflow: scroll;
  }
  /*スマホサイズに適用*/
  @media screen and (max-width:599px){
    .content {
      height: calc(100vh - 140px);
      overflow: scroll;
      margin-bottom: 100px;
    }
  }
</style>
