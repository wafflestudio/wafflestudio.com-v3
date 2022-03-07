<script lang="ts">
  import Banner from './components/banner/banner.svelte';
  import About from './components/description/about/about.svelte';
  import Member from './components/description/member.svelte';
  import Organization from './components/organization/organization.svelte';
  import RecruitLink from './components/recruit-link/recruit-link.svelte';
  import Activity from './components/description/activity.svelte';
  import Schedule from './components/schedule/schedule.svelte';
  import Footer from './components/footer/footer.svelte';

  export let name: string;
</script>

<main>
  <h1>Hello {name}!</h1>
  <p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
  <Banner />
  <About />
  <Member />
  <Organization />
  <RecruitLink />
  <Activity />
  <Schedule />
  <Footer />
</main>

<style>
  main {
    text-align: center;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
