<script>
	import Github from '$lib/icons/companies/Github.svelte';
	export let iconSize = 'h-6 w-6 sm:w-8 sm:h-8';
	import { appState } from '$lib/utils/appState';
</script>

<a
	class="flex items-center space-x-6 tracking-wider text-zinc-100 hover:text-neutral md:px-4 text-xl md:text-2xl font-normal normal-case "
	href="https://github.com/cornucopia-rs/cornucopia"
>
	<Github class="{iconSize} text-white opacity-80 hover:text-white hover:scale-105 " />
	{#if $appState.screenSize === 'Small'}
		<h1>Go to Github</h1>
	{/if}
</a>
