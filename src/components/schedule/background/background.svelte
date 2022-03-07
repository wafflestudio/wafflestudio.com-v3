<div class="tablecloth">
  <div />
  <img class="trident" src="images/trident.png" alt="background fork" />
  <img class="sword" src="images/sword.png" alt="background knife" />
</div>

<style>
  div.tablecloth {
    position: absolute;
    width: 1200px;
    height: 500px;
    box-sizing: border-box;
    top: calc(50vh - 240px);
    left: calc(50vw - 600px);
    background-color: #986259;
    padding-top: 130px;
  }

  div.tablecloth > div {
    height: 240px;
    width: 100%;
    background-color: #f4987b;
  }

  img {
    height: 600px;
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
