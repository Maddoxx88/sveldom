<script>
  import { goto } from '$app/navigation';
  import "../styles/buttons.css";
  // your script goes here
  const handleClick = () => {
  console.log("clicked");
};

</script>

<!-- Main navigation container -->
<nav
  class="flex w-full items-center justify-between bg-transparent py-2 lg:justify-start lg:py-4 px-12"
  data-te-navbar-ref>
  <div class="flex w-full flex-wrap items-center justify-between">
    <!-- Hamburger button for mobile view -->
    <h1 class="text-3xl text-white font-bold">Sveldom</h1>

    <div class="flex w-96 justify-between">
      <h2 class="text-white font-medium p-2">Home</h2>
      <h2 class="text-white p-2">New</h2>
      <h2 class="text-white p-2">Top</h2>
      <h2 class="text-white p-2">About</h2>
    </div>

    <!-- Right elements -->
    <div class="relative flex items-center">
      <button class="pushable-white mr-2" on:click={() => goto(`/signin`) }>
        <span class="shadow-white"></span>
        <span class="edge-white"></span>
        <span class="front-white">Sign In</span>
      </button>
      <button class="pushable ml-2" on:click={() => goto(`/register`) }>
        <span class="shadow"></span>
        <span class="edge"></span>
        <span class="front">Sign up</span>
      </button>

    </div>
  </div>
</nav>
