<script>
    import '../../styles/buttons.css';
    import GameCard from './game-card.svelte';
    // your script goes here
    let games = [
		{ id: '1', name: 'Typescrisis', url: 'typecrisis' },
		{ id: '2', name: 'Flash Out', url: 'flash-out' },
		{ id: '3', name: 'Trigger Fingers', url: 'trigger-fingers' }
	];
</script>

<div class="bg-[#4062ff] grid grid-cols-3 grid-flow-row"> 
	{#each games as { id, name, url }, i}
		<GameCard name={name} url={url} />
	{/each}
</div> 

       