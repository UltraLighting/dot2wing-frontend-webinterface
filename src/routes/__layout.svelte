<!-- load page path -->
<script context="module">
  export const load = async ({ page }) => ({
    props: {
      key: page.path,
    },
  })
</script>
<script>
  import Version from '../components/version.svelte';
  import PageTransition from '../components/PageTransition.svelte'
  // import Nav from '../components/navGhost.svelte';
  export let key
</script>
<svelte:head>
  <title>Wing Dashboard</title>
</svelte:head>
<!-- <Nav /> -->
<!-- make page transistion -->
<PageTransition refresh={key}>
  <slot />
  <Version />
</PageTransition>
<style>
  :global(body) { background-color: #1d1d1d; }
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>