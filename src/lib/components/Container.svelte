<div class="container"><slot /></div>

<style>
  .container {
    margin: 0 auto;
    padding-top: 4px;
    padding-bottom: 24px;
    /* height: 100vh;
    overflow-y: scroll; */
  }
  .container::-webkit-scrollbar{
    display: none;
  }
</style>
