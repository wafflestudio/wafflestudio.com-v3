<section>
  <dl>
    <dt class="outer">준회원</dt>
    <dd class="outer">
      <p>
        루키즈는 운영팀이 주관하는 세미나 과정 (세미나 + 토이프로젝트) 을 훌륭히 이수할 경우 정회원 중 <strong
          >programmer 로 승격</strong
        >하게 돼요.
      </p>
    </dd>

    <dt class="outer">정회원</dt>
    <dd class="outer">
      <p>
        활동회원일 경우 <strong
          >github push 권한, notion 편집 권한, aws IAM, 그리고 와플스튜디오가 제공하는 코딩 모임 • 스프린트 지원금 수령의 권한</strong
        >을 얻게 돼요. 즉, 프로젝트나 스터디 등 와플스튜디오의 활동에 참여하기 위해서는 반드시 활동회원이어야겠죠? 😀
      </p>
    </dd>

    <dt class="inner">디자이너</dt>
    <dd class="inner">
      <p>
        미술대학 디자인과 학생이 아니더라도 디자인에 관심이 있으면 디자이너가 될 수 있어요.<br />Ps, Ai 정도만 다룰 수 있다면
        Figma, Sketch, XD 등의 툴은 금세 익힐 수 있어요! (프로젝트마다 사용하는 툴이 달라요)
      </p>
    </dd>

    <dt class="inner">프로그래머</dt>
    <dd class="inner">
      <p>
        분야는 크게 <strong>프론트 • 백 • 안드로이드 • iOS</strong> 네 가지로 나뉘어요.<br />팀 빌딩때 초기 멤버로 참여하거나,
        이미 진행 중인 프로젝트에 충원 인력으로 들어갈 수 있어요.<br />관심있는 분야의 스터디에도 참여할 수 있어요.
      </p>
    </dd>

    <dt class="inner">운영팀</dt>
    <dd class="inner">
      <p>
        운영팀은 와플스튜디오의 <strong>모든 운영을 맡아서 진행</strong>해요.<br />리크루팅, 팀빌딩, 인프라 관리, 프로젝트 관리,
        회원 관리, 재정 관리, 외부 컨택 등이요!
      </p>
    </dd>

    <dt class="inner dark">비활동회원</dt>
    <dd class="inner dark">
      <p>
        한번 정회원 자격을 얻으면 별다른 일이 있지 않다면 계속 정회원 자격을 유지하게 돼요.<br /><strong>비활동 회원</strong>은
        활동을 쉬고 있는 회원이에요. 상 / 하반기 마다 해당 기간에 활동하실 건지에 대한 신청을 받아요.
      </p>
    </dd>
  </dl>
</section>

<style>
  section {
    width: 100vw;
    height: 100vh;
    background-color: #0b4c4f;
  }

  p {
    margin: 0;
  }

  dl {
    padding-top: calc(50vh - 360px);
    margin: 0 auto;
    width: 1200px;
    height: 700px;
    display: grid;
    grid-template-columns: 150px 150px auto;
    gap: 20px;
  }

  dt {
    width: 150px;
    height: 100px;
    line-height: 100px;
    background-color: #196164;
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    letter-spacing: -0.05em;
    color: #ffffff;
  }

  dt:first-of-type,
  dd:first-of-type {
    margin-bottom: 28px;
  }

  dd {
    font-style: normal;
    font-weight: 300;
    font-size: 16px;
    background-color: #196164;
    line-height: 26px;
    align-items: center;
    letter-spacing: -0.05em;
    text-align: left;
    color: #ffffff;
    margin: 0;
    padding: 10px 30px 10px 20px;
    display: flex;
    align-items: center;
  }

  dt.outer {
    grid-column-start: 1;
    grid-column-end: 2;
  }
  dt.inner {
    grid-column-start: 2;
    grid-column-end: 3;
  }

  dd.outer {
    grid-column-start: 2;
    grid-column-end: 4;
  }
  dd.inner {
    grid-column-start: 3;
    grid-column-end: 4;
  }

  .dark {
    background-color: #123d40;
  }
</style>
