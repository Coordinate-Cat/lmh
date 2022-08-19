<div class="content"><slot /></div>

<style>
  .content {
    margin: 4px;
    border: 1px solid #000;
  }
  /*スマホサイズに適用*/
  @media screen and (max-width:599px){
    .content {
      margin-bottom: 60px;
    }
  }
</style>
