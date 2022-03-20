<script>
  import ProjectWrapper from '../common/project-wrapper/project-wrapper.svelte';
  import Overview from '../common/overview/overview.svelte';
  import Carousel from '../common/carousel/carousel.svelte';
</script>

<ProjectWrapper class="project-gatgu-wrapper" id={'gatgu'}>
  <Overview
    logo={'../../../images/gatgu.png'}
    name={'같이구매'}
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
  :global(.project-gatgu-wrapper) {
    background: radial-gradient(35.89% 41.81% at 50% 53.89%, #ffffff 0%, #ffdc48 100%);
    border: 25px solid #274e8c;
    box-sizing: border-box;
    color: #6e6363;
  }
</style>
