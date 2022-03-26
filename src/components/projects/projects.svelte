<script lang="ts">
  import Banner from './banner.svelte';

  let current: 'snuboard' | 'snutt' | 'shiksha' = 'snuboard';
</script>

<section id="projects">
  <h3 class="title">출시된 프로젝트</h3>
  <div class="circles">
    <div class="circle" />
    <div class="circle" />
    <div class="circle" />
    <div class="circle" />
  </div>

  <div class="line-left" />
  <div class="line-right" />

  <div class="waffle-studio">
    <span>waffle</span>
    <span>studio</span>
  </div>

  <div class="wrapper">
    <div class="project">
      {#if current === 'snutt'}
        <img src="https://cdn.pixabay.com/photo/2015/11/06/15/14/service-1028805_960_720.jpg" alt="" class="pc" />
      {:else}
        <img src="/assets/main/mobile.png" alt="" />
      {/if}
    </div>
    <ul class="icons">
      <li
        class="
    icon"
        on:click={() => (current = 'snuboard')}
      >
        <img src="/assets/main/snuboard.svg" alt="" />
        <span>스누보드</span>
      </li>
      <li
        class="
      icon"
        on:click={() => (current = 'snutt')}
      >
        <img src="/assets/main/snutt.svg" alt="" />
        <span>SNUTT</span>
      </li>
      <li
        class="
      icon"
        on:click={() => (current = 'shiksha')}
      >
        <img src="/assets/main/snutt.svg" alt="" />
        <span>식샤</span>
      </li>
      <li
        class="
      icon"
        on:click={() => (current = 'snuboard')}
      >
        <img src="/assets/main/snuboard.svg" alt="" />
        <span>???</span>
      </li>
    </ul>
  </div>
</section>
<Banner />

<style>
  #projects {
    width: 100%;
    height: 100vh;
    background: #342d29;
    position: relative;
    overflow: hidden;
  }

  #projects .circles {
    position: absolute;
    top: 130px;
    left: -29px;
  }

  #projects .circles .circle {
    display: inline-block;
    margin: 0 -20px;
    width: 116px;
    height: 116px;
    border-radius: 50%;
    background: rgba(255, 241, 207, 0.05);
  }

  #projects h3.title {
    font-style: normal;
    font-weight: bold;
    font-size: 24px;
    line-height: 25px;
    letter-spacing: -0.05em;
    color: #fff1cf;

    position: absolute;
    top: 156px;
    left: 252px;
  }

  #projects div.line-left {
    border: 2px solid rgba(255, 241, 207, 0.2);
    transform: rotate(-10deg);
    position: absolute;
    top: 50%;
    left: -10vw;
    width: 20vw;
  }

  #projects div.line-right {
    border: 2px solid rgba(255, 241, 207, 0.2);
    transform: rotate(-10deg);
    position: absolute;
    top: 27%;
    right: -10vw;
    width: 20vw;
  }

  #projects div.waffle-studio {
    width: 100%;
    height: 200px;
    font-family: Lobster;
    font-style: normal;
    font-weight: normal;
    font-size: 150px;

    background: linear-gradient(269.88deg, #5b5247 3.58%, #ed8573 98.67%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;

    position: absolute;
    top: 30%;
    transform: translateY(-0%) rotate(-10deg);
    text-align: center;
  }

  #projects div.waffle-studio span {
    font-family: Lobster;
    margin: 130px;
  }

  #projects div.wrapper {
    display: flex;
    flex-direction: column;
    gap: 41px;

    width: 100%;
    height: 100%;
    align-items: center;
    justify-content: center;
  }

  #projects div.wrapper div.project {
    position: relative;
    height: 550px;
    width: 800px;
    max-height: 550px;
    z-index: 5;
  }

  #projects div.wrapper div.project img {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  #projects div.wrapper div.project img.pc {
    width: 800px;
    height: 500px;

    background: #5b5247;
    border: 10px solid #fff1cf;
    box-sizing: border-box;
    border-radius: 18px;
    z-index: 5;
  }

  #projects div.wrapper ul {
    display: flex;
    gap: 21px;
    list-style: none;
    padding: 0;
    margin: 0;
  }

  #projects div.wrapper ul li.icon {
    list-style: none;
    cursor: pointer;

    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 12px;
  }

  #projects div.wrapper ul.icons li.icon img {
    width: 81px;
    height: 81px;
    list-style: none;
    border-radius: 10px;
  }

  #projects div.wrapper ul.icons li.icon span {
    font-size: 20px;
    font-style: normal;
    font-weight: 300;
    line-height: 18px;
    letter-spacing: -0.05em;
    text-align: center;
    color: #fff1cf;
  }
</style>
