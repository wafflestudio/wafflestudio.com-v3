<script lang="ts">
  import type { Key } from '../../banner';
  import LightOff from '../../assets/light-off.svg.svelte';
  import LightOn from '../../assets/light-on.svg.svelte';

  export let key: Key, label: string, current: Key;
  export let setCurrent: (key: Key) => void;

  $: active = key === current;
</script>

<menuitem href={key} on:click={() => setCurrent(key)}>
  {#if active}
    <LightOn />
  {:else}
    <LightOff />
  {/if}

  <span class={active && 'active'}>{label}</span>
</menuitem>

<style>
  menuitem {
    width: 174px;
    height: 307.75px;
    position: relative;
    cursor: pointer;
  }

  span {
    position: absolute;
    bottom: 0;
    width: 100%;
    text-align: center;
    left: 0;
    color: #181105;
    font-size: 18px;
    line-height: 20px;
    font-weight: 300;
    height: 30px;
    transition: 0.3s color;
  }

  menuitem:hover span {
    color: #ffd260;
  }

  span::before {
    content: '';
    position: absolute;
    left: 0;
    right: 0;
    height: 3px;
    bottom: -3px;
    background: #ffd260;
    opacity: 0;
    transition: 0.4s opacity;
  }

  menuitem:hover span::before {
    opacity: 0.8;
  }

  span.active {
    font-weight: 500;
    line-height: 21px;
    color: #ffd260;
  }

  span.active::before {
    opacity: 1;
  }
</style>
