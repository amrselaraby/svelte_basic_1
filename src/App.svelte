<script>
	import Button from './lib/Button.svelte'
	import FaAngellist from 'svelte-icons/fa/FaAngellist.svelte'
	import FaAllergies from 'svelte-icons/fa/FaAllergies.svelte'
</script>

<Button on:click|once={() => alert(true)} let:isLeftHover size="large" shadow disabled>
	<div style:width="20px" slot="leftContent">
		{#if isLeftHover}
			<FaAngellist />
		{:else}
			<FaAllergies />
		{/if}
	</div>
	Some Text
</Button>

<style>
</style>
