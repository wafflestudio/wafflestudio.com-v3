<script>
  import Content from './content.svelte';

  let currentMonth = new Date().getMonth() + 1;

  const monthItems = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12].map((month) => {
    const left = Math.sin((month * Math.PI) / 6) * 240 + 275;
    const top = Math.cos(((month + 6) * Math.PI) / 6) * 240 + 275;
    return {
      label: month,
      style: `left: ${left}px; top: ${top}px`,
    };
  });
</script>

<article>
  {#each monthItems as monthItem, i}
    <div
      class="month"
      class:activeMonth={currentMonth === i + 1}
      style={monthItem.style}
      on:mouseenter={() => (currentMonth = monthItem.label)}
    >
      {monthItem.label}
    </div>
  {/each}
  <Content {currentMonth} />
</article>

<style>
  article {
    position: absolute;
    border-radius: 50%;
    width: 600px;
    height: 600px;
    left: calc(50% - 300px);
    top: calc(50% - 310px);
    background-color: #ffe4ae;
  }

  .month {
    font-family: 'Lobster';
    font-size: 50px;
    position: absolute;
    width: 50px;
    height: 50px;
  }

  .activeMonth {
    background-color: white;
  }
</style>
