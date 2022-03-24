<script lang="ts">
  import NavigateItem from './navigate-item/navigate-item.svelte';
  import type { Key } from '../banner';

  const links: { key: Key; label: string }[] = [
    { key: 'wafflestudio', label: '와플스튜디오' },
    { key: 'instagram', label: '인스타그램' },
    { key: 'recruit', label: '신입생 모집' },
    { key: 'service', label: '앱 출시' },
  ];

  export let current: Key;
  export let setCurrent: (key: Key) => void;
</script>

<menu>
  {#each links as { key, label }}
    <NavigateItem {key} {label} {current} {setCurrent} />
  {/each}
</menu>

<style>
  menu {
    display: inline-flex;
    gap: 42px;
    margin: 0 auto;
    border-bottom: 3px solid #181105;
  }
</style>
