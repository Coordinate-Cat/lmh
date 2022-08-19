<div class="content"><slot /></div>

<style>
  .content {
    margin: 4px;
    margin-bottom: 0;
    border: 1px solid #000;
    height: 100%;
    overflow: scroll;
  }
  /*スマホサイズに適用*/
  @media screen and (max-width:599px){
    .content {
      height: 100%;
      overflow: scroll;
      /* margin-bottom: 60px; */
    }
  }
</style>
