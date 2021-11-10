<script>
  export let name;
  export let type;
  export let reach;
  const style = 'p-6 bg-black text-gray-300 text-center rounded-md shadow-md flex flex-col items-center';
</script>
{#if type === 'fader'}
  <p class="{style}">{type}</p>
{:else if type === 'number'}
  <p class="{style}">{type}</p>
{:else if type === 'switch'}
  <p class="{style}">{type}</p>
{:else}
  <p class="{style}">Setting not defined: {type? type:'type missing'}</p>
{/if}
