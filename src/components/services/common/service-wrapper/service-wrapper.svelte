<script lang="ts">
  let className: string;
  export { className as class };
  export let id: string;
</script>

<section {id} class={className}>
  <slot />
</section>

<style>
  section {
    width: 100vw;
    height: 100vh;
    scroll-snap-align: start;
    position: relative;
    display: flex;
    flex-direction: column;
    gap: 10px;
    align-items: center;
    justify-content: center;
  }
</style>
