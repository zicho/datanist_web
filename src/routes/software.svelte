<script context="module">
	export async function preload(page, session) {
		const res = await this.fetch(`../software.json`);
		const software = await res.json();
		console.log(software)
		return { software };
	}
</script>

<script>
	import SoftwareCard from '../components/SoftwareCard.svelte'
	export let software
	console.log(software)
</script>

<svelte:head>
	<title>datanist</title>
</svelte:head>

<div class="page test">
	<h2>Software</h2>
	<h5>
		On this page you can find a list of software, frameworks and such that I enjoy
		using.
	</h5>
	<hr />
	{#if software}
	{#each software as s}
		<SoftwareCard {...s} />
	{/each}
	{/if}
</div>
