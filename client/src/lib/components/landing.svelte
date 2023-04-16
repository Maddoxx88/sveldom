<script>
    import '../../styles/buttons.css';
    // your script goes here
    const handleClick = () => {
    console.log("clicked");
  };
</script>

<div class="flex mx-12 my-8">
    <div class="flex flex-col mx-4 w-2/3 gap-8">
        <h1 class="text-9xl font-bold text-white">Online Mobile Games</h1>
        <button class="pushable ml-2 w-96" on:click={() => handleClick()}>
            <span class="shadow"></span>
            <span class="edge"></span>
            <span class="front">Sign up and play &rsaquo;</span>
          </button>
    </div>
    <div class="flex-1 w-80"></div>
    <div class="flex">
        <img src="https://images.unsplash.com/photo-1518895312237-a9e23508077d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1484&q=80" alt="">
    </div>
</div>
