<svelte:head>
	<title>datanist</title>
</svelte:head>
<div class="page test">
	<br />
	<div class="resp-container">
		<iframe
			title="game"
			class="resp-iframe"
			src="https://game.datanist.se"
			gesture="media"
			allow="encrypted-media"
			allowfullscreen />
	</div>
</div>

<style>
	.resp-container {
		position: relative;
		overflow: hidden;
		padding-top: 56.25%;
	}

	.resp-iframe {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		border: 0;
	}
</style>
