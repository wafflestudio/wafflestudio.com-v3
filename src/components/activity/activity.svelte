<script lang="ts">
  let current: string = '';

  const images = {
    project: '/assets/main/activity-seminar.png',
    seminar: '/assets/main/activity-seminar-2.png',
    coding: '/assets/main/activity-seminar.png',
    waffle: '/assets/main/activity-seminar-2.png',
    study: '/assets/main/activity-seminar.png',
  };

  const changeCurrent = (key: string) => {
    current = key;
  };
</script>

<section class="main-activity">
  <div class="circles">
    <div class="circle" />
    <div class="circle" />
    <div class="circle" />
    <div class="circle" />
  </div>

  <h3 id="title">주요 활동</h3>

  <p class="description">2주간 진행한 프로젝트 내용을 간단하게 발표하고 <br />의견을 나누는 행사입니다.</p>

  <ul class="activity-items">
    <li class="item" class:active={current === 'project'}>
      <p on:mouseenter={() => changeCurrent('project')}>프로젝트</p>
    </li>
    <li class="item r-60" class:active={current === 'seminar'}>
      <p on:mouseenter={() => changeCurrent('seminar')}>루키 세미나</p>
    </li>
    <li class="item l-66" class:active={current === 'coding'}>
      <p on:mouseenter={() => changeCurrent('coding')}>코딩 모임</p>
    </li>
    <li class="item l-40 active" class:active={current === 'waffle'}>
      <p on:mouseenter={() => changeCurrent('waffle')}>와플 반죽하기 · 굽기</p>
    </li>
    <li class="item r-34" class:active={current === 'study'}>
      <p on:mouseenter={() => changeCurrent('study')}>스터디</p>
    </li>
  </ul>

  <img class="l-10 t-50" src={images[current] || images.project} alt="" width="30%" />
  <img class="r-10 t-30" src="/assets/main/activity-seminar-2.png" alt="" width="25%" />
  <img class="r-6 t-46 " src="/assets/main/activity-seminar.png" alt="" width="25%" height="300px" />
</section>

<style>
  .main-activity {
    position: relative;
    height: 100vh;
    background: #0b4c4f;
  }

  .main-activity .circles {
    position: absolute;
    top: 108px;
    left: -29px;
  }

  .main-activity .circles .circle {
    display: inline-block;
    margin: 0 -20px;
    width: 116px;
    height: 116px;
    border-radius: 50%;
    background: rgba(255, 241, 207, 0.05);
  }

  .main-activity #title {
    position: absolute;
    top: 155px;
    left: 16%;
    margin: 0;

    font-style: normal;
    font-weight: 700;
    font-size: 24px;

    letter-spacing: -0.05em;

    color: #fff1cf;
  }

  .main-activity p {
    margin: 0;
  }

  .main-activity p.description {
    margin: 0;
    text-align: left;
    display: inline-block;
    width: fit-content;

    position: absolute;
    top: 392px;
    left: 10%;

    font-style: normal;
    font-weight: 300;
    font-size: 20px;
    line-height: 24px;

    color: #fff1cf;
  }

  .main-activity ul {
    padding: 0;
    margin: 0;
    list-style: none;
  }

  .main-activity ul.activity-items {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    display: flex;
    flex-direction: column;
  }

  .main-activity ul.activity-items li.item {
    position: relative;

    font-style: normal;
    font-size: 70px;
    font-weight: 400;
    line-height: 80px;
    letter-spacing: -0.05em;
    text-align: center;
    color: #fff1cf99;

    cursor: default;
  }

  .main-activity ul.activity-items li.item.r-60 {
    right: 60px;
  }

  .main-activity ul.activity-items li.item.l-66 {
    left: 66px;
  }

  .main-activity ul.activity-items li.item.l-40 {
    left: 40px;
  }

  .main-activity ul.activity-items li.item.r-34 {
    right: 34px;
  }

  .main-activity ul.activity-items li.item p {
    display: inline-block;
    width: fit-content;

    font-family: 'KCC-eunyoung' !important;
  }

  .main-activity ul.activity-items li.item.active p {
    color: #fff1cf;
    background: repeating-linear-gradient(#00000000, #00000000 25px, #d56c2a 25px, #d56c2a 55px);
  }

  .main-activity img {
    border: 3px solid #fff1cf;
    background: rgba(255, 241, 207, 0.3);
    box-sizing: border-box;
    position: absolute;
  }

  .main-activity img.l-10.t-50 {
    top: 50%;
    left: 10%;
  }

  .main-activity img.r-10.t-30 {
    top: 30%;
    right: 10%;
  }

  .main-activity img.r-6.t-46 {
    top: 46%;
    right: 6%;
  }
</style>
