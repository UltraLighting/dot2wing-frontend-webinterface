<script>
  import Version from '../components/version.svelte';
</script>
<svelte:head>
  <title>Wing Dashboard</title>
</svelte:head>
<slot></slot>
<Version/>
<style>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>