<script lang="ts">
  export let logo: string;
  export let name: string;
  export let description: string;

  export let links: {
    android: string;
    iOS: string;
    web: string;
  };
</script>

<div class="wrapper">
  <img src={logo} alt={name} width={145} />
  <div class="content">
    <h1 class="name">{name}</h1>
    <p class="description">{description}</p>
  </div>
  <nav class="links">
    <a class="linkItem" href={links.iOS}>
      <img src={'../../../images/app-store.png'} alt={'app store link'} width={45} />
    </a>
    <a class="linkItem" href={links.android}>
      <img src={'../../../images/play-store.png'} alt={'app store link'} width={45} />
    </a>
    <a class="linkItem" href={links.web}>
      <img src={'../../../images/web.png'} alt={'app store link'} width={45} />
    </a>
  </nav>
</div>

<style>
  .wrapper {
    width: 864px;
    height: 145px;
    box-sizing: border-box;
    padding-inline-start: 115px;
    padding-inline-end: 100px;
    display: flex;
    gap: 25px;
    z-index: 99;
  }

  .content {
    width: 345px;
  }

  .name {
    font-weight: 700;
    font-size: 30px;
    line-height: 34.5px;
    letter-spacing: -3px;
    margin-bottom: 4px;
    margin-top: 16px;
  }

  .description {
    font-weight: 300;
    font-size: 18px;
    line-height: 20.7px;
    letter-spacing: -1.8px;
    white-space: pre-line;
    height: 100px;
    margin: 16px 0 0 0;
  }

  .links {
    width: 150px;
    display: flex;
    gap: 7.5px;
    padding-top: 70px;
  }

  .linkItem {
    width: 45px;
    height: 45px;
  }
</style>
