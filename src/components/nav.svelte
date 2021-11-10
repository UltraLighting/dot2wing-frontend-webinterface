<script>
  export let title;
  export let loggedOut;
  function handleLogout() {
    alert('placeholder: logout');
  }
</script>

<nav class=" bg-black shadow-xl sticky top-0 z-50">
  <div class="max-w-6xl mx-auto px-4 flex justify-between">
    <div class="flex space-x-7">
      <!-- logo and title -->
      <div class="flex items-center py-4 px-2">
        <img src="./favicon.png" alt="Logo" class="h-8 w-8 mr-4 invert">
        <span class="font-semibold text-gray-300 text-lg uppercase">{title || ''}</span>
      </div>
    </div>
    <!-- display logout button -->
    {#if !loggedOut}
    <div class="md:flex items-center">
      <a on:click={handleLogout} href= "/" class="py-2 px-2 font-medium text-white bg-red-500 rounded hover:bg-red-600 transition duration-200">Log out</a>
    </div>
    {/if}
  </div>
</nav>