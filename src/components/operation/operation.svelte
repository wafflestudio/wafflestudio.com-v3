<section class="operation">
  <div class="phone">
    <div class="talk">
      <div class="header">
        <span class="title">푸푸리</span>
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

  .operation .phone .talk span {
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

  .operation .phone .talk span::before {
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
</style>
