<script>
  import Nav from '../components/nav.svelte';
</script>
<Nav title="Welcome to your wing!" loggedOut=true/>
<!-- login page -->
<div class="flex w-full mt-40">
  <form class="m-auto bg-black shadow-md rounded-md px-8 pt-6 pb-8 mb-6">
    <div class="mb-6">
      <label class="block text-gray-400 text-sm font-bold mb-2 uppercase" for="password">pin</label>
      <div class="flex w-full">
        <input maxlength="1" min="0" class="shadow w-10 mx-2 appearance-none border border-red-500 rounded py-2 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline">
        <input maxlength="1" min="0" class="shadow w-10 mx-2 appearance-none border border-red-500 rounded py-2 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline">
        <input maxlength="1" min="0" class="shadow w-10 mx-2 appearance-none border border-red-500 rounded py-2 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline">
        <input maxlength="1" min="0" class="shadow w-10 mx-2 appearance-none border border-red-500 rounded py-2 text-gray-700 mb-3 leading-tight focus:outline-none focus:shadow-outline">
      </div>
        <p class="text-red-500 text-xs italic">Wrong PIN.</p>
    </div>
    <div class="flex justify-center">
      <a class="bg-gray-400 hover:bg-gray-700 text-white font-bold py-2 px-4 rounded uppercase" href="/dashboard">
        Login
      </a>
    </div>
  </form>
</div>