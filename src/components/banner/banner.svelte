<script lang="ts">
  import Navigator from './navigator/navigator.svelte';
  import type { Key } from './carousel';

  let current: Key = 'wafflestudio';

  const setCurrent = (key: Key) => (current = key);

  $: link = (() => {
    switch (current) {
      case 'wafflestudio':
        return 'https://yt3.ggpht.com/ytc/AKedOLSZmhVSQtTtir5RU8Pi-7y_K84BP9ij7HzJHEM=s900-c-k-c0x00ffffff-no-rj';
      case 'instagram':
        return 'https://blog.kakaocdn.net/dn/CHb0U/btqxrW04Y5b/mzimBHhLuGMBYvCS33uyh0/img.jpg';
      case 'recruit':
        return 'https://learningspoons-lms-s3.s3.amazonaws.com/media/course/techrecruiting/%ED%85%8C%ED%81%AC%EB%A6%AC%ED%81%AC%EB%A3%A8%ED%8C%85_%EC%8D%B8%EB%84%A4%EC%9D%BC-min_2.png';
      case 'service':
        return 'https://cdn.pixabay.com/photo/2015/11/06/15/14/service-1028805_960_720.jpg';
    }
  })();
</script>

<section>
  <Navigator {current} {setCurrent} />
  <br />
  <img src={link} alt={current} />
</section>

<style>
  section {
    background: #5b5247;
    height: 100vh;
    text-align: center;
  }

  img {
    width: 864px;
    height: 486px;
    object-fit: cover;
    display: inline-block;
    margin-top: 20px;
  }
</style>
