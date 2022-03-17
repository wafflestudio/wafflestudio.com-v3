<div class="tablecloth">
  <div />
  <img class="trident" src="images/trident.png" alt="background fork" />
  <img class="sword" src="images/sword.png" alt="background knife" />
</div>

<style>
  div.tablecloth {
    position: absolute;
    width: 1000px;
    height: 400px;
    box-sizing: border-box;
    top: calc(50vh - 210px);
    left: calc(50vw - 500px);
    background-color: #986259;
    padding-top: 100px;
  }

  div.tablecloth > div {
    height: 200px;
    width: 100%;
    background-color: #f4987b;
  }

  img {
    height: 500px;
    position: absolute;
    top: -30px;
  }

  img.trident {
    left: 60px;
  }

  img.sword {
    right: 60px;
  }
</style>
