<script>
	import { AppBar } from '@skeletonlabs/skeleton';
	import Palete from '../components/palete.svelte';
	let paletes = [
		{
			name: 'palete 1',
			colors: [
				'#006466',
				'#065A60',
				'#0B525B',
				'#144552',
				'#1B4332',
				'#212F45',
				'#272640',
				'#312244',
				'#3E1F47',
				'#4A1942',
			]
		}
	]
</script>

<AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end">
	<svelte:fragment slot="lead"></svelte:fragment>
	<h1>Colors :)</h1>
	
</AppBar>
<div class="container">
	{#each paletes as palete}
		<Palete name={palete.name} colors={palete.colors} />
	{/each}
</div>