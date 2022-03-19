<section class="operation">
  <div class="phone">
    <div class="talk">
      <div class="header">
        <span class="title">푸푸리</span>
      </div>
      <div class="contents">
        <div class="speech-bubble left">
          <p>오 !</p>
        </div>
        <div class="speech-bubble right">
          <p>와플 스튜디오 노션에 초대받으면 노션을 이용해 팀 활동</p>
          <p>내용을 정리하고 진행할 수 있어요</p>
        </div>
        <div class="speech-bubble right">
          <p>새 프로젝트의 개발을 시작하면 와플 스튜디오 깃허브에서</p>
          <p>새 레포지토리의 어드민 권한을 받을 수 있어요!</p>
        </div>
        <div class="speech-bubble right">
          <p>와플스튜디오 정회원이 되면 슬랙에 초대 받게돼요!</p>
          <p>슬랙에는 주제별로 다양한 채널이 존재한답니다.</p>
        </div>
        <div class="speech-bubble left">
          <p>#와플 스튜디오 내부 운영 방식이 궁금해요!</p>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
  .operation {
    position: relative;
    background: #c55743;
    height: 100vh;
  }

  .operation .phone {
    position: absolute;
    left: 200px;
    bottom: 0;

    width: 780px;
    height: 900px;

    background: #1b1b1b;
    border-radius: 55px 55px 0 0;
  }

  .operation .phone .talk {
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);

    height: 800px;
    width: 730px;

    background: #c55743;
  }

  .operation .phone .talk .header {
    position: relative;
    background: #9a4747;
    vertical-align: middle;
    height: 90px;
  }

  .operation .phone .talk .header span {
    display: inline-block;
    position: absolute;
    top: 50%;
    left: 90px;
    transform: translateY(-50%);

    font-style: normal;
    font-weight: 500;
    font-size: 24px;
    line-height: 28px;

    color: #ffffff;
  }

  .operation .phone .talk .header span::before {
    content: '';
    display: block;
    width: 40px;
    height: 28px;

    background: url('/assets/common/left-arrow.svg') center no-repeat;

    position: absolute;
    top: 0;
    left: -60px;
  }

  .operation .phone .talk span::after {
    content: '';
    display: block;
    width: 28px;
    height: 28px;

    background: url('/assets/common/waffle.svg') center no-repeat;

    position: absolute;
    top: 0;
    right: -34px;
  }

  .operation .phone .talk .contents {
    width: 100%;
    position: absolute;
    bottom: 0;
    padding: 0 20px 50px 45px;
    box-sizing: border-box;

    display: flex;
    flex-direction: column-reverse;
    gap: 50px;
  }
  .operation .phone .talk .contents .speech-bubble {
    position: relative;
    padding: 15px 20px;
    width: fit-content;
    background: #702e2e;
    border-radius: 23px;
  }

  .operation .phone .talk .contents .speech-bubble.left {
    margin-left: 100px;
  }

  .operation .phone .talk .contents .speech-bubble.left::before {
    content: '';
    width: 106px;
    height: 106px;

    position: absolute;
    left: -120px;
    top: -10px;

    background: url('/assets/common/pupuri.svg') center no-repeat;

    z-index: -1;
  }

  .operation .phone .talk .contents .speech-bubble.left::after {
    content: '';
    width: 0;
    height: 0;

    position: absolute;
    bottom: -20px;

    border: 20px solid;
    border-color: transparent transparent transparent #702e2e;
    transform: rotate(10deg);
    z-index: -1;
  }

  .operation .phone .talk .contents .speech-bubble.right {
    align-self: flex-end;
  }

  .operation .phone .talk .contents .speech-bubble.right::after {
    content: '';
    width: 0;
    height: 0;

    position: absolute;
    bottom: -20px;
    right: 20px;

    border: 20px solid;
    border-color: transparent #702e2e transparent transparent;
    transform: rotate(-10deg);
    z-index: 1;
  }
  .operation .phone .talk .contents .speech-bubble p {
    margin: 0;

    font-size: 18px;
    font-style: normal;
    font-weight: 300;
    line-height: 21px;
    letter-spacing: 0em;
    text-align: left;
    color: #ffffff;
  }
</style>
