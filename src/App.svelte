<script lang="ts">
  import Footer from './components/footer/footer.svelte';
  import Projects from './components/projects/projects.svelte';
  export let name: string;
</script>

<main>
  <Projects />
  <Footer />
</main>

<style>
  main {
    text-align: center;
    max-width: 240px;
    margin: 0 auto;
  }


  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
