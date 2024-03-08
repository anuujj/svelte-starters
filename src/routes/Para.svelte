<script>
  let counter = 0;
  function increment() {
    counter += 1;
  }
  function decrement() {
    counter -= 1;
  }
  export let description;
</script>

<p>para from another component</p>
<p>{description}</p>
<div>
  <button on:click={increment}>+</button>
  <span>Count = {counter}</span>
  <button on:click={decrement}>-</button>
  {#if counter > 10}
    <p>Count is really high</p>
  {:else if counter > 0}
    <p>count is positive</p>
  {:else}
    <p>count is really low</p>
  {/if}
</div>
