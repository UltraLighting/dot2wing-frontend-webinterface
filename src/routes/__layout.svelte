<script>
  import Nav from '../components/nav.svelte';
</script>
<svelte:head>
  <title>UltraLighting Dashboard</title>
</svelte:head>
<Nav/>
<slot></slot>
<style>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>