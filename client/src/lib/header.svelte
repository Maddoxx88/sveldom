<!-- Main navigation container -->
<nav
  class="flex-no-wrap relative flex w-full items-center justify-between bg-transparent py-2 lg:flex-wrap lg:justify-start lg:py-4"
  data-te-navbar-ref>
  <div class="flex w-full flex-wrap items-center justify-between px-3">
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
      <button class="pushable-white mr-2" on:click={() => handleClick()}>
        <span class="shadow-white"></span>
        <span class="edge-white"></span>
        <span class="front-white">Sign In</span>
      </button>
      <button class="pushable ml-2" on:click={() => handleClick()}>
        <span class="shadow"></span>
        <span class="edge"></span>
        <span class="front">Sign up</span>
      </button>

    </div>
  </div>
</nav>

<style>
.pushable {
    position: relative;
    border: none;
    background: transparent;
    padding: 0;
    cursor: pointer;
    outline-offset: 4px;
    transition: filter 250ms;
  }
  .shadow {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 25px;
    background: hsl(0deg 0% 0% / 0.25);
    will-change: transform;
    transform: translateY(2px);
    transition: transform 600ms cubic-bezier(0.3, 0.7, 0.4, 1);
  }
  .edge {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 25px;
    background: linear-gradient(
      to left,
      hsl(34deg 100% 16%) 0%,
      hsl(34deg 100% 32%) 8%,
      hsl(34deg 100% 32%) 92%,
      hsl(34deg 100% 16%) 100%
    );
  }
  .front {
    display: block;
    position: relative;
    padding: 12px 42px;
    border-radius: 25px;
    font-size: 1.25rem;
    color: white;
    background: #f78d1d;
    background: -webkit-gradient(
      linear,
      left top,
      left bottom,
      from(#ffc260),
      to(#f47a20)
    );
    /* background: hsl(39deg, 100%, 50%); */
    will-change: transform;
    transform: translateY(-4px);
    transition: transform 600ms cubic-bezier(0.3, 0.7, 0.4, 1);
    text-transform: uppercase;
    font-family: "Satoshi", sans-serif;
    font-weight: bold;
  }
  /* .pushable:hover {
    filter: brightness(80%);
  } */
  .pushable:hover .front {
    transform: translateY(-6px);
    transition: transform 250ms cubic-bezier(0.3, 0.7, 0.4, 1.5);
  }
  .pushable:active .front {
    transform: translateY(-2px);
    transition: transform 34ms;
  }
  .pushable:hover .shadow {
    transform: translateY(4px);
    transition: transform 250ms cubic-bezier(0.3, 0.7, 0.4, 1.5);
  }
  .pushable:active .shadow {
    transform: translateY(1px);
    transition: transform 34ms;
  }
  .pushable:focus:not(:focus-visible) {
    outline: none;
  }
  
  .pushable-white {
    position: relative;
    border: 1px solid rgba(255, 255, 255, 0.5);
    border-radius: 25px;
    background: transparent;
    padding: 0;
    cursor: pointer;
    outline-offset: 4px;
    transition: filter 250ms;
  }
  .shadow-white {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 25px;
    background: transparent;
    will-change: transform;
    transform: translateY(2px);
    transition: transform 600ms cubic-bezier(0.3, 0.7, 0.4, 1);
  }
  .edge-white {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 25px;
    background: transparent;
  }
  .front-white {
    display: block;
    position: relative;
    padding: 12px 42px;
    border-radius: 25px;
    font-size: 1.25rem;
    color: white;
    border: 1px solid rgba(255, 255, 255, 0.5);
    background: #5d7aff;
    /* background: hsl(39deg, 100%, 50%); */
    will-change: transform;
    transform: translateY(-4px);
    transition: transform 600ms cubic-bezier(0.3, 0.7, 0.4, 1);
    text-transform: uppercase;
    font-family: "Satoshi", sans-serif;
    font-weight: bold;
  }
  /* .pushable:hover {
    filter: brightness(80%);
  } */
  .pushable-white:hover .front-white {
    transform: translateY(-6px);
    transition: transform 250ms cubic-bezier(0.3, 0.7, 0.4, 1.5);
    background: white;
    color: #5d7aff;
  }
  .pushable-white:active .front-white {
    transform: translateY(-2px);
    transition: transform 34ms;
  }
  .pushable-white:hover .shadow-white {
    transform: translateY(4px);
    transition: transform 250ms cubic-bezier(0.3, 0.7, 0.4, 1.5);
  }
  .pushable-white:active .shadow-white {
    transform: translateY(1px);
    transition: transform 34ms;
  }
  .pushable-white:focus:not(:focus-visible) {
    outline: none;
  }
  
  .sign-in-btn {
    border: 1px solid white;
  }
  
</style>

<script>
    // your script goes here
    const handleClick = () => {
    console.log("clicked");
  };
</script>