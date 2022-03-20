<script lang="ts">
  export let current: number;

  export let items: {
    label: string;
    anchor: string;
  }[];
</script>

<nav class="wrapper" class:hide={current < 0}>
  {#each items as item, i}
    <a class="linkItem" href={`#${item.anchor}`}>
      <span class="linkText">{item.label}</span>
      <span class="bullet" class:selected={current === i}>&nbsp;</span>
    </a>
  {/each}
</nav>

<style>
  .wrapper {
    position: fixed;
    right: 55px;
    top: calc(50vh - 84px);
    width: 145px;
    height: 166px;
    z-index: 999;
    display: flex;
    flex-direction: column;
    gap: 9px;
    opacity: 1;
    transition: opacity 0.3s;
  }

  .wrapper.hide {
    opacity: 0;
  }

  .linkItem {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 26px;
    text-decoration: none;
  }

  .linkText {
    font-style: normal;
    text-decoration: none;
    font-weight: 500;
    font-size: 15px;
    line-height: 17px;
    display: inline-block;
    align-items: center;
    text-align: right;
    letter-spacing: -0.1em;
    color: #ffffff;
    width: 118px;
  }

  .bullet {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    border: 1.5px solid #ffffff;
    box-sizing: border-box;
    transition: background-color 0.3s;
  }
  .bullet.selected {
    background-color: #ffffff;
  }
</style>
