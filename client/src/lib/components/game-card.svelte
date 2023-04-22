<script>
    // your script goes here
    /**
	 * @type {String}
	 */
     export let name;
     /**
	 * @type {String}
	 */
      export let url;
</script>

<div class="m-4 h-fit">
    <div class="flex mx-12 my-8 hover:scale-105">
        <div class="flex bg-[#2e44b9]">
            <img src="https://images.unsplash.com/photo-1518895312237-a9e23508077d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1484&q=80" class="w-56" alt="">
        </div>
        <div class="flex flex-col mx-4 w-2/3 gap-8">
            <h1 class="text-2xl font-bold text-white">{name}</h1>
            <button class="w-24 bg-[#f78d1d] px-8 py-2 hover:drop-shadow-[5px_5px_15px_rgba(247,141,29,0.5)] border-x-0 border-t-0 border-b-4 border-b-orange-700 uppercase text-white">
                <a href='/{url}'>Play</a>
              </button>
        </div>
    </div>
  </div>