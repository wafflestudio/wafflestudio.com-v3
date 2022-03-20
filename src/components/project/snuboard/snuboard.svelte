<script>
  import ProjectWrapper from '../common/project-wrapper/project-wrapper.svelte';
  import Overview from '../common/overview/overview.svelte';
  import Carousel from '../common/carousel/carousel.svelte';
</script>

<ProjectWrapper class="project-snuboard-wrapper" id={'snuboard'}>
  {#each Array(8) as _}
    <div class="bgItem" />
  {/each}

  <Overview
    logo={'../../../images/snuboard.png'}
    name={'스누보드'}
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
  :global(.project-snuboard-wrapper) {
    background-color: #42b8df;
    color: #ffffff;
  }

  .bgItem {
    width: 33%;
    height: 14%;
    position: absolute;

    background: linear-gradient(270.19deg, #3988d1 0.17%, rgba(57, 136, 209, 0) 101.6%);
    border-radius: 0 75px 75px 0;
  }

  .bgItem:nth-of-type(1) {
    top: 2.8%;
    left: 1.7%;
  }
  .bgItem:nth-of-type(2) {
    top: 2.8%;
    left: 30%;
  }
  .bgItem:nth-of-type(3) {
    top: 19%;
    left: -10%;
  }
  .bgItem:nth-of-type(4) {
    top: 19%;
    left: 48%;
  }
  .bgItem:nth-of-type(5) {
    top: 35%;
    left: -1%;
  }
  .bgItem:nth-of-type(6) {
    top: 51%;
    left: -20%;
  }
  .bgItem:nth-of-type(7) {
    top: 67%;
    left: 66%;
  }
  .bgItem:nth-of-type(8) {
    top: 83%;
    left: 51%;
  }
</style>
