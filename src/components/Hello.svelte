<script>
  const message = 'Svelte';

  let isSvelte = true;

  const updateText = () => {
    isSvelte = !isSvelte;
  };
</script>

{#if isSvelte}
  <h1>Hello {message}!</h1>
{:else}
  <h1>Hello Astro!</h1>
{/if} 

<button on:click={updateText}>Update!</button>
