<script>
  import Background from './background/background.svelte';
  import Calendar from './calendar/calendar.svelte';
</script>

<section>
  <Background />
  <Calendar />
</section>

<style>
  section {
    background-color: #7e473e;
    width: 100vw;
    height: 100vh;
    position: relative;
    overflow: hidden;
  }
</style>
