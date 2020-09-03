<script>
	import Nav from '../components/Nav.svelte'

	export let segment
</script>

<Nav {segment} />

<main>
	<slot />
</main>

<style>
	main {
		position: relative;
		background-color: white;
		box-sizing: border-box;
		margin: var(--margin-xxl) var(--margin-xs);
	}

	@media (min-width: 1200px) {
		main {
			margin: var(--margin-l) var(--margin-xxl);
		}
	}
</style>
