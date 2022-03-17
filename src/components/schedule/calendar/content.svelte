<script lang="ts">
  import { contents } from './content';
  export let currentMonth: string;
</script>

<section>
  <h3>#와플스튜디오는 매주 토요일마다!</h3>
  <div>
    <span>{currentMonth}월</span>
    <dl>
      {#each Object.entries(contents[currentMonth]) as [week, activities]}
        <dt>{week}주</dt>
        <dd>
          {#each activities as activity}
            <p>{activity}</p>
          {/each}
        </dd>
      {/each}
    </dl>
  </div>
</section>

<style>
  section {
    position: absolute;
    width: 320px;
    left: calc(50% - 160px);
    top: 200px;
  }

  h3 {
    color: #7e473e;
    font-weight: 700;
    font-size: 22px;
    line-height: 30px;
    letter-spacing: -0.05em;
  }

  div {
    display: flex;
    gap: 20px;
  }

  span {
    width: 72px;
    height: 32px;
    background: #c55743;
    color: #fff1cf;
    font-weight: 700;
    font-size: 20px;
    line-height: 30px;
    text-align: center;
    letter-spacing: -0.05em;
    border-radius: 10px;
  }

  dl {
    display: grid;
    grid-template-columns: 36px auto;
    gap: 20px 0;
    margin: 0;
  }

  dt {
    font-style: normal;
    font-weight: 700;
    font-size: 16px;
    line-height: 20px;
    letter-spacing: -0.05em;
    color: #342d29;
  }

  dd {
    margin: 0;
  }

  p {
    margin: 0;
    text-align: left;
    font-family: 'Gmarket Sans TTF';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 20px;
    letter-spacing: -0.05em;
    color: #7e473e;
  }
</style>
