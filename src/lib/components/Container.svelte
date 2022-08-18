<div class="container"><slot /></div>

<style>
  .container {
    max-width: 768px;
    margin: 0 auto;
    height: 100%;
    overflow-y: scroll;
  }
  .container::-webkit-scrollbar{
    display: none;
  }
</style>
