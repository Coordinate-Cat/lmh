<div class="container"><slot /></div>

<style>
  .container {
    /* width: 760px; */
    margin: 0 auto;
    /* padding: 0 200px; */
    height: 100%;
    overflow-y: scroll;
  }
  .container::-webkit-scrollbar{
    display: none;
  }
</style>
