<script>
  import Address from './address/address.svelte';
  import Light from './assets/light.svg.svelte';
  import Keyboard from './keyboard/keyboard.svelte';
</script>

<footer>
  <Keyboard />
  <Light />
  <Address />
</footer>

<style>
  footer {
    width: calc(100% - 63px);
    height: 738px;
    background: #342d29;
    position: relative;
    text-align: left;
    padding-inline-start: 63px;
  }
</style>
