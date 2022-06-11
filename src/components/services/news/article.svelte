<script lang="ts">
  export let src: string;
  export let alt: string;
</script>

<article>
  <img {src} {alt} />
</article>

<style>
  article,
  article img {
    width: 365px;
    height: 365px;
  }
</style>
