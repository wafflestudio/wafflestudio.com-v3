<script lang="ts">
  import Banner from '../components/banner/banner.svelte';
  import About from '../components/description/about/about.svelte';
  import Member from '../components/description/member.svelte';
  import MainActivity from '../components/activity/activity.svelte';
  import Organization from '../components/organization/organization.svelte';
  import RecruitLink from '../components/recruit-link/recruit-link.svelte';
  import Activity from '../components/description/activity.svelte';
  import Schedule from '../components/schedule/schedule.svelte';
  import Footer from '../components/footer/footer.svelte';
  import Cover from '../components/cover/cover.svelte';
  import Operation from '../components/operation/operation.svelte';
</script>

<main>
  <Cover />
  <Banner />
  <About />
  <Member />
  <Organization />
  <MainActivity />
  <RecruitLink />
  <Activity />
  <Schedule />
  <Operation />
  <Footer />
</main>
