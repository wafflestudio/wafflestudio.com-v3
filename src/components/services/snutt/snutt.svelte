<script>
  import ProjectWrapper from '../common/service-wrapper/service-wrapper.svelte';
  import Overview from '../common/overview/overview.svelte';
  import Carousel from '../common/carousel/carousel.svelte';
</script>

<ProjectWrapper class="project-snutt-wrapper" id="snutt">
  {#each Array(7) as _}<div class="timeItem">&nbsp;</div>{/each}
  <Overview
    logo="../../../images/snutt.png"
    name="SNUTT"
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
  :global(.project-snutt-wrapper) {
    color: #6e6363;
  }

  .timeItem {
    width: 9%;
    min-width: 100px;
    background-color: #4e642d;
    position: absolute;
  }

  .timeItem:nth-of-type(1) {
    height: 338px;
    background-color: #e54459;
    left: 20px;
    top: 20px;
  }

  .timeItem:nth-of-type(2) {
    height: 579px;
    background-color: #1bd0c8;
    left: 20px;
    top: 378px;
  }

  .timeItem:nth-of-type(3) {
    height: 460px;
    background-color: #a6d930;
    left: calc(max(9%, 100px) + 40px);
    top: 196px;
  }

  .timeItem:nth-of-type(4) {
    height: 404px;
    background-color: #f58d3d;
    left: calc(max(9%, 100px) + 40px);
    top: 676px;
  }

  .timeItem:nth-of-type(5) {
    height: 60%;
    background-color: #fac42d;
    right: calc(max(9%, 100px) + 40px);
    bottom: 20%;
  }

  .timeItem:nth-of-type(6) {
    height: 60%;
    background-color: #2bc267;
    right: 20px;
    top: 0;
  }

  .timeItem:nth-of-type(7) {
    height: 37.4%;
    background-color: #af56b3;
    right: 20px;
    bottom: 0;
  }
</style>
