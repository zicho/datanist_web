<script>
	import Nav from '../components/Nav.svelte'

	export let segment
</script>

<Nav {segment} />

<main class="screen-padding-right screen-padding-left">
	<slot />
</main>

<style>
	main {
		position: relative;
		background-color: white;
		box-sizing: border-box;
	}
</style>
