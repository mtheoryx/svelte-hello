<script>
  let count = 0;
  let clicks = 0;
  $: doubled = count * 2;
  function handleIncrement() {
    count++;
    clicks++;
  }
  function handleDecrement() {
    count--;
    clicks++;
  }
</script>

<style>
  p {
    color: red;
  }
</style>

<button on:click={handleIncrement}> + </button>
<span>{doubled}</span>
<span>{count == 0 ? 'Time' : 'Times'}</span>
<button on:click={handleDecrement}> - </button>
<hr />
<p>
  <span>You have clicked Shiny things {clicks}
    {clicks == 1 ? 'Time' : 'Times'}</span>
</p>
