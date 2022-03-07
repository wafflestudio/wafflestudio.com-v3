<section>
  <dl>
    <dt class="outer">준회원</dt>
    <dd class="outer">asdf</dd>

    <dt class="outer">정회원</dt>
    <dd class="outer">asdf</dd>

    <dt class="inner">디자이너</dt>
    <dd class="inner">asdf</dd>

    <dt class="inner">프로그래머</dt>
    <dd class="inner">asdf</dd>

    <dt class="inner">운영팀</dt>
    <dd class="inner">asdf</dd>

    <dt class="inner">비활동회원</dt>
    <dd class="inner">asdf</dd>
  </dl>
</section>

<style>
  section {
    width: 100vw;
    height: 100vh;
    background-color: #0b4c4f;
  }

  dl {
    padding-top: calc(50vh - 360px);
    margin: 0 auto;
    width: 1000px;
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

  dd {
    font-style: normal;
    font-weight: 300;
    font-size: 18px;
    background-color: #196164;
    line-height: 30px;
    align-items: center;
    letter-spacing: -0.05em;
    color: #ffffff;
    margin: 0;
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
</style>
