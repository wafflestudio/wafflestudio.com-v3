<script>
  import Cover from '../cover/cover.svelte';

  import Navigator from './common/navigator/navigator.svelte';
  import Gatgu from './gatgu/gatgu.svelte';
  import Guam from './guam/guam.svelte';
  import Siksha from './siksha/siksha.svelte';
  import Snuboard from './snuboard/snuboard.svelte';
  import Snutt from './snutt/snutt.svelte';
  import News from './news/news.svelte';

  import { throttle } from 'lodash';

  let current = 0;

  const projectItems = [
    { label: 'SNUTT', anchor: 'snutt' },
    { label: '식샤', anchor: 'siksha' },
    { label: '스누보드', anchor: 'snuboard' },
    { label: 'GUAM', anchor: 'guam' },
    { label: '같이구매', anchor: 'gatgu' },
  ];

  const handleScroll = throttle((e) => {
    current = Math.round(e.target.scrollTop / window.innerHeight - 1);
  }, 100);
</script>

<main class="wrapper" on:scroll={handleScroll}>
  <Cover current="services" />
  <Navigator {current} items={projectItems} />
  <Snutt />
  <Siksha />
  <Snuboard />
  <Guam />
  <Gatgu />
  <News />
</main>

<style>
  .wrapper {
    height: 100vh;
    overflow-y: scroll;
    overflow-x: hidden;
  }
</style>
