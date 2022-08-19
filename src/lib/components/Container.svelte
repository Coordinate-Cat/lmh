<div class="container"><slot /></div>

<style>
  .container {
    margin: 0 auto;
    height: 100vh;
    overflow-y: scroll;
  }
  .container::-webkit-scrollbar{
    display: none;
  }
</style>
