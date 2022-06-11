<script>
  import Article from './article.svelte';
</script>

<section id="news">
  <h3><span>와플스튜디오의 가장 빠른 소식을 인스타그램에서 만나보세요.</span></h3>
  <div class="news-article">
    <Article src="/assets/tmp/shiksha.png" />
    <Article src="/assets/tmp/snuboard.png" />
    <Article src="/assets/tmp/shiksha.png" />
    <Article src="/assets/tmp/snuboard.png" />
    <Article src="/assets/tmp/shiksha.png" />
    <Article src="/assets/tmp/snuboard.png" />
    <Article src="/assets/tmp/shiksha.png" />
    <Article src="/assets/tmp/snuboard.png" />
    <Article src="/assets/tmp/shiksha.png" />
    <Article src="/assets/tmp/snuboard.png" />
    <Article src="/assets/tmp/shiksha.png" />
    <Article src="/assets/tmp/snuboard.png" />
  </div>
  <div class="marquee">
    <div class="track">
      <p>
        #괌 #스누데이 #스누그 #샤틀버스 #스타피커 #클린코드 스터디 #코루틴 스터디 #괌 #스누데이 #스누그 #샤틀버스 #스타피커
        #클린코드 스터디 #코루틴 스터디
      </p>
    </div>
  </div>
</section>

<style>
  section#news {
    width: 100%;
    height: 100vh;

    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  section#news h3 {
    width: 100%;
    text-align: center;
    border-bottom: 1px solid #342d29;
    line-height: 0;
    margin: 0 0 90px;
  }

  section#news h3 span {
    background: #fff;
    padding: 0 20px;
    color: #342d29;

    font-size: 24px;
    font-weight: 500;
    /* line-height: 28px; */
    /* letter-spacing: -0.05em; */
    text-align: center;
  }

  section#news div.news-article {
    width: 100%;
    height: fit-content;
    overflow-x: scroll;

    display: flex;
    flex-direction: row;

    gap: 56px;
  }

  section#news div.marquee {
    position: relative;
    width: 100%;
    max-width: 100%;
    height: 70px;
    overflow-x: hidden;

    margin-top: 70px;
  }

  section#news div.marquee div.track {
    position: absolute;
    white-space: nowrap;
    will-change: transform;
    animation: marquee 16s linear infinite;
  }

  section#news div.marquee div.track p {
    font-family: 'Gmarket Sans TTF';
    font-size: 48px;
    font-weight: 300;
    line-height: 55px;

    margin: 0;
  }

  @keyframes marquee {
    from {
      transform: translateX(0);
    }
    to {
      transform: translateX(-50%);
    }
  }
</style>
