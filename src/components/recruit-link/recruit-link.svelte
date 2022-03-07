<section>
  <p>와플스튜디오에 대해 더 알고 싶으신가요?</p>
  <a href="/recruit">
    모집 안내 보기
    <svg xmlns="http://www.w3.org/2000/svg" width="12" height="24" viewBox="0 0 16 25" fill="none">
      <path d="M2 23L13 12.6019L2 2" stroke="#ED8573" stroke-width="4" />
    </svg>
  </a>

  <div />
  <div />
  <div />
  <div />
</section>

<style>
  section {
    display: flex;
    align-items: center;
    gap: 54px;
    height: 140px;
    justify-content: center;
    background: linear-gradient(0deg, #fff1cf, #fff1cf), linear-gradient(90deg, #ed8573 0%, #f0975e 100%);
    position: relative;
  }

  p {
    font-weight: 500;
    font-size: 28px;

    display: flex;
    align-items: center;
    letter-spacing: -0.05em;
    margin: 0;
    color: #342d29;
  }

  a {
    display: block;
    width: 220px;
    height: 50px;
    line-height: 26px;
    gap: 8px;
    text-decoration: none;
    font-weight: bold;
    font-size: 26px;
    letter-spacing: -0.05em;
    display: flex;
    align-items: center;
    justify-content: center;

    color: #ed8573;
    border: 4px solid #ed8573;
    box-sizing: border-box;
    border-radius: 10px;
    transition: 0.3s all;
    background-color: transparent;
  }

  div {
    position: absolute;
    width: 300px;
    height: 140px;
    top: 0;

    border-radius: 30px;
    transform: rotate(-180deg);
    transform: skewX(12deg);
  }

  div:nth-of-type(1) {
    background: #9d8476;
    left: -50px;
  }
  div:nth-of-type(2) {
    background: #6e6363;
    left: -120px;
  }
  div:nth-of-type(3) {
    background: #9d8476;
    right: -50px;
  }
  div:nth-of-type(4) {
    background: #6e6363;
    right: -120px;
  }

  section > div {
    transition: 0.2s all;
  }

  section:hover > div {
    width: 280px;
  }

  section:hover > a {
    box-shadow: 0 0 4px #ed8573;
    background-color: #ed857320;
  }
</style>
