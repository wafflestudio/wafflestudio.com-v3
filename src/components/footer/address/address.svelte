<script>
  import Instagram from '../assets/instagram.svg.svelte';
  import Mail from '../assets/mail.svg.svelte';
</script>

<address>
  <div class="address-item">
    <Instagram />
    <div class="instagram-link">
      <h4 class="label">와플스튜디오 인스타그램</h4>
      <a target="_blank" href="https://www.instagram.com/wafflestudio_official/">@wafflestudio_official</a>
    </div>
  </div>
  <div class="address-item">
    <Mail />
    <ul>
      <li class="mail-link-item">
        <h4 class="label">총괄 및 문의</h4>
        <p class="email" data-clipboard-text="master@wafflestudio.com">master@wafflestudio.com</p>
      </li>
      <li class="mail-link-item">
        <h4 class="label">리크루팅 지원</h4>
        <p class="email" data-clipboard-text="recruit@wafflestudio.com">recruit@wafflestudio.com</p>
      </li>
      <li class="mail-link-item">
        <h4 class="label">와플 동아리장</h4>
        <p class="email" data-clipboard-text="woohm404@wafflestudio.com">woohm404@wafflestudio.com</p>
      </li>
    </ul>
  </div>
</address>

<style>
  address {
    font-style: normal;
    position: absolute;
    bottom: 62px;
    left: 104px;
  }

  div.address-item {
    display: flex;
    gap: 45px;
    align-items: center;
    margin-top: 58px;
  }

  div.instagram-link h4 {
    width: 300px;
  }

  ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  li.mail-link-item {
    display: flex;
    align-items: center;
    margin: 4px 0;
  }

  h4.label {
    width: 140px;
    font-weight: 700;
    font-size: 20px;
    line-height: 23px;
    color: #fff1cf;
    margin: 0;
  }

  p.email {
    font-weight: 300;
    font-size: 24px;
    line-height: 27px;
    color: #fff1cf;
    margin: 0;
    cursor: pointer;
  }
</style>
