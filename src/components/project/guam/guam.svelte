<script>
  import ProjectWrapper from '../common/project-wrapper/project-wrapper.svelte';
  import Overview from '../common/overview/overview.svelte';
  import Carousel from '../common/carousel/carousel.svelte';
</script>

<ProjectWrapper class="project-guam-wrapper" id={'guam'}>
  {#each Array(8) as _}
    <div class="bgItem" />
  {/each}
  <Overview
    logo="../../../images/guam.png"
    name={'GUAM'}
    description={'SNUTT는 서울대학교 시간표 어플입니다.\nSNUTT는 서울대학교 대표 시간표 어플입니다.\nSNUTT는 서울대학교 시간표 어플입니다.'}
    links={{ android: '', iOS: '', web: '' }}
  />
  <Carousel
    imageList={[
      'https://static.smilegatemegaport.com/live/game/2dc9bd7ede8c40a39ec9d436e831a032.png',
      'https://www.meconomynews.com/news/photo/202106/55023_65722_4627.jpg',
      'https://w.namu.la/s/ee4b3696c69829fb8acb96a8a6b666363f599c21fdffd4501a0e5b1187d8676e4ea9fce6dfd7a328ef7f055b4ce3e6feaad9f6c4df9d3b5e8ef7a3482bca63b037b280cf9c83d140910e2457ab9581fa',
    ]}
  />
</ProjectWrapper>

<style>
  :global(.project-guam-wrapper) {
    color: #6e6363;
  }

  .bgItem {
    position: absolute;
  }

  .bgItem:nth-of-type(1) {
    width: 500px;
    height: 200px;
    left: 0;
    top: 0;

    background: rgba(131, 111, 255, 0.5);
    border-radius: 0 0 200px 200px;
  }

  .bgItem:nth-of-type(2) {
    width: 400px;
    height: 200px;
    left: 308px;
    top: 0;

    background: rgba(254, 141, 159, 0.5);
    border-radius: 0 0 200px 200px;
  }

  .bgItem:nth-of-type(3) {
    width: 600px;
    height: 300px;
    right: 0;
    bottom: 0;

    background: #aeffba;
    border-radius: 200px 200px 0 0;
  }

  .bgItem:nth-of-type(4) {
    width: 300px;
    height: 400px;
    right: 0;
    bottom: 0;

    background: rgba(131, 111, 255, 0.5);
    border-radius: 200px 0 0 200px;
  }

  .bgItem:nth-of-type(5) {
    width: 300px;
    height: 900px;
    right: 0;
    bottom: 0;

    background: rgba(131, 111, 255, 0.5);
    border-radius: 200px 0 0 200px;
  }

  .bgItem:nth-of-type(6) {
    width: 400px;
    height: 200px;
    left: 0;
    bottom: 0;

    background: rgba(139, 255, 156, 0.5);
    border-radius: 200px 200px 0 0;
  }

  .bgItem:nth-of-type(7) {
    width: 600px;
    height: 200px;
    left: 0;
    bottom: 0;

    background: rgba(255, 231, 124, 0.5);
    border-radius: 200px 200px 0 0;
  }

  .bgItem:nth-of-type(8) {
    width: 200px;
    height: 500px;
    left: 0;
    bottom: 0;

    background: rgba(254, 141, 159, 0.5);
    border-radius: 0 200px 0 0;
  }
</style>
