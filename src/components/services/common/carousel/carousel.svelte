<script lang="ts">
  import Arrow from './arrow.svelte';

  export let imageList: string[];
  let index = 0;
</script>

<div class="wrapper">
  <img class="mainImage" src={imageList[index]} alt="snutt" />
  <div class="imageSelector">
    <button on:click={() => (index = (index - 1 + imageList.length) % imageList.length)}><Arrow /></button>
    {#each imageList as item, i}
      <img class="imageItem" src={item} alt="snutt" onClick={() => (index = i)} />
    {/each}
    <button class="arrow" on:click={() => (index = (index + 1) % imageList.length)}><Arrow /></button>
  </div>
</div>

<style>
  .wrapper {
    width: 45vw;
    height: 57vh;
    z-index: 99;
  }

  .mainImage {
    width: 100%;
    height: 45vh;
    margin: 0;
    object-fit: contain;
  }

  .imageSelector {
    margin-top: 14px;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 9px;
  }

  .imageItem {
    width: 11vw;
    height: 11vh;
    margin: 0;
    object-fit: cover;
  }

  .arrow {
    margin: 0 10px;
    cursor: pointer;
  }

  .arrow:last-child {
    transform: rotate(180deg);
  }

  button {
    background: transparent;
    border: none;
  }
</style>
