<script lang="ts">
  export let current: '' | 'services' | 'members';
</script>

<section class="main">
  <h1>
    <a href="/">
      <span>와플스튜디오</span>
      <img src="/assets/common/logo.svg" alt="logo" />
    </a>
  </h1>

  <a href="/recruting" id="recruting">
    <span>동아리 모집안내</span>
    <img src="/assets/common/recruting.svg" alt="recruting" />
  </a>

  <img src="/assets/common/full_logo.svg" alt="full_logo" id="full-logo" />

  <nav>
    <ul>
      <li class:active={current === ''}>
        <a href="/">소개</a>
      </li>
      <li class:active={current === 'services'}>
        <a href="/services">서비스</a>
      </li>
      <li class:active={current === 'members'}>
        <a href="/members">멤버</a>
      </li>
    </ul>
  </nav>

  <div class="description">
    <p>
      와플스튜디오는 서울대학교 컴퓨터공학부 웹 / 앱 개발 동아리입니다.
      <br /> 타과생도 동아리에 지원하실 수 있습니다.
    </p>
  </div>

  <div id="background">
    <p>WAFFLE</p>
    <p>STUDIO</p>
    <p>WAFFLE</p>
  </div>
</section>

<style>
  .main {
    height: 100vh;
    position: relative;
  }

  .main a span {
    display: none;
  }

  .main h1 {
    position: absolute;
    top: 65px;
    left: 73px;
  }

  .main #recruting {
    position: absolute;
    top: 69px;
    right: 60px;
  }

  .main #full-logo {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  .main #background {
    width: 100%;
    text-align: center;

    padding: 40px 0;
  }

  .main #background p {
    margin: 0;

    font-family: 'nico-moji-regular', sans-serif;
    font-size: 360px;
    font-style: normal;
    font-weight: 400;
    line-height: 225px;
    letter-spacing: 0.1em;
    color: #fdf2dc4a;
  }

  .main nav {
    width: 670px;
    position: absolute;
    left: 50%;
    bottom: 160px;
    transform: translateX(-50%);
  }

  .main nav ul {
    margin: 0;
    padding: 0;
    display: flex;
    list-style: none;
  }

  .main nav ul li {
    display: inline-block;
    width: calc(100% / 3);
    height: 44px;

    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    letter-spacing: -0.15em;
    text-align: center;
    color: #f0975e;
  }

  .main nav ul li a {
    display: inline-block;
    width: 100%;
    height: 100%;
    line-height: 44px;

    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    letter-spacing: -0.15em;
    text-align: center;
    vertical-align: middle;
    color: #f0975e;
  }

  .main nav ul li a:hover {
    text-decoration: none;
  }

  .main nav ul li.active {
    background-color: #fedb96;
  }

  .main nav ul li.active a {
    color: #791930;
  }

  .main .description {
    width: 100%;
    position: absolute;
    bottom: 40px;

    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: 21px;
    letter-spacing: -0.1em;
    text-align: center;
    color: #791930;
  }
</style>
