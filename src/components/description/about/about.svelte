<section class="about">
  <div class="circle w-254 t-145 l-145" />
  <div class="circle w-198 t-443 r-57" />
  <div class="circle w-129 b-90 r-496" />
  <div class="circle striped w-298 t-328 l-71" />
  <div class="circle striped w-420 b-152 r-100" />

  <article class="description">
    <h3>#와플스튜디오는 어떤 동아리인가요?</h3>
    <hr />
    <p>
      와플스튜디오는 서울대학교 컴퓨터공학부에서 탄생한 <b>웹 / 앱 개발 동아리</b>예요.
    </p>
    <p>와플스튜디오는 개발자들의 커뮤니티 형성을 도모하고, 개발에 대해 서로 이야기하고 경험하며 성장하는 것을 추구해요.</p>
    <br />
    <p>
      🖥️  와플스튜디오에서는 이런 성장을 위해 여러 가지 활동이 진행돼요. 대표적으로 <b>프로젝트</b>가 있어요.
    </p>
    <p>개발자라면 많은 경우 결국 프로젝트를 하는 직업이 되기 때문에, 프로젝트 진행은 와플스튜디오에서 가장 큰 활동이에요.</p>
    <p>
      아니면 개발과 관련하여 원하는 주제가 있다면 자유롭게 <b>스터디</b>를 열 수도 있어요. 프로젝트든 스터디든, 근본적인 목적은
      “개발 공부” 랍니다!
    </p>
    <br />
    <p>
      🗣️ 또한 개발자간의 커뮤니티를 도모하기 위해 “<b>코딩 모임</b>”이라는 모임이 매월 + 자유롭게 열려요.
    </p>
    <p>코딩을 좋아하는 사람들끼리 모여서 각자 할 일을 하게 돼요.</p>
    <p>
      그러면서 코딩이나 개발과 관련된 이야기도 나누고, <b>친목</b>을 다질 수 있어요!
    </p>
  </article>
</section>

<style>
  .about {
    height: 100vh;
    background: #342d29;
    position: relative;
  }

  .about .description {
    position: absolute;
    width: 100%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    color: #fff1cf;
    font-style: normal;
    letter-spacing: -0.05em;
    text-align: center;
  }

  .about .description h3 {
    font-size: 22px;
    font-weight: 700;
  }

  .about .description p {
    font-size: 18px;
    font-weight: 300;
  }

  .about .description p b {
    font-weight: 500;
  }

  .about .description hr {
    border: none;
    content: '';
    margin: 2em;
    display: block;
    font-size: 100%;
  }

  .about .description br {
    content: '';
    margin: 2em;
    display: block;
    font-size: 150%;
  }

  .about .circle {
    background: #fff1cf0d;
    position: absolute;
    border-radius: 50%;
  }

  .about .circle.w-254.t-145.l-145 {
    width: 254px;
    height: 254px;
    top: 145px;
    left: 145px;
  }

  .about .circle.w-198.t-443.r-57 {
    width: 198px;
    height: 198px;
    top: 443px;
    right: 57px;
  }

  .about .circle.w-129.b-90.r-496 {
    width: 129px;
    height: 129px;
    bottom: 90px;
    right: 496px;
  }

  .about .circle.striped {
    background: repeating-linear-gradient(-10deg, #fff1cf0d, #fff1cf0d 6px, #00000000 6px, #00000000 24px);
  }

  .about .circle.striped.w-298.t-328.l-71 {
    width: 298px;
    height: 298px;
    top: 328px;
    left: 71px;
  }

  .about .circle.striped.w-420.b-152.r-100 {
    width: 420px;
    height: 420px;
    bottom: 152px;
    right: 100px;
  }
</style>
