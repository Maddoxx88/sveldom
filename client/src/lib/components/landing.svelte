<script>
    import '../../styles/buttons.css';
    // your script goes here
    const handleClick = () => {
    console.log("clicked");
  };
</script>

<div class="flex flex-col justify-center mx-12 my-8 h-[36rem] max-h-max" id="landing-section">
    <div class="flex my-4 mx-4 gap-8">
        <h1 class="text-9xl font-bold font-inter mx-auto text-white">Online Svelte Games</h1>
    </div>
    <div class="my-8 mx-auto"> 
        <button class="pushable w-96" on:click={() => handleClick()}>
            <span class="shadow"></span>
            <span class="edge"></span>
            <span class="front font-inter">Play Now &rsaquo;</span>
          </button>
    </div>
</div>