<script context="module" lang="ts">
	export async function preload(page, session) {
		console.log('preload!', page, session)
	}
</script>

<script lang="ts">
	// import { onMount } from 'svelte'
	// import { writable } from 'svelte/store'

	// import Counter from '@app/components/Counter.svelte'

	// const count = writable(100)

	// onMount(() => {
	// 	console.log('App mounted')
	// })
</script>

<svelte:head>
	<title>datanist</title>
</svelte:head>

<div class="page test">
	<h1>Welcome to <span style="color: black">datanist</span></h1>
	<hr />
	<p>
		This is a personal site with no real purpose. It will
		mainly serve as a testing ground for SPA/SSR websites and various
		applications using
		<a href="https://svelte.dev/">Svelte</a>
		and
		<a href="https://sapper.svelte.dev/">Sapper</a>
		. It can also be used to contact me about various projects, some of which
		can be found on my
		<a href="https://github.com/zicho">github page</a>
		.
	</p>
</div>
