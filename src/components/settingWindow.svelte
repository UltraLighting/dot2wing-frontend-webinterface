<script>
  export let name;
  export let type;
  export let reach;
  const style = 'transition duration-50 ease-in-out p-6 bg-gray-100 text-gray-800 text-center rounded-md shadow-sm hover:shadow-md flex flex-col items-center';
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
