<script>
	import Card from 'sveltestrap/src/Card.svelte'
	import CardHeader from 'sveltestrap/src/CardHeader.svelte'
	import CardTitle from 'sveltestrap/src/CardTitle.svelte'
	import CardBody from 'sveltestrap/src/CardBody.svelte'
	import CardSubtitle from 'sveltestrap/src/CardSubtitle.svelte'
	import CardText from 'sveltestrap/src/CardText.svelte'
</script>

<svelte:head>
	<title>datanist</title>
</svelte:head>

<div class="page test">
	<h2>Software I like</h2>
	<Card>
		<CardHeader>
			<CardTitle>Card title</CardTitle>
		</CardHeader>
		<CardBody>
			<CardSubtitle>Card subtitle</CardSubtitle>
			<CardText>
				Some quick example text to build on the card title and make up the bulk
				of the card's content.
			</CardText>
		</CardBody>
	</Card>
</div>
