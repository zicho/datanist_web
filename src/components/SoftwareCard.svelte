<script lang="ts">
	import Card from 'sveltestrap/src/Card.svelte'
	import CardHeader from 'sveltestrap/src/CardHeader.svelte'
	import CardTitle from 'sveltestrap/src/CardTitle.svelte'
	import CardBody from 'sveltestrap/src/CardBody.svelte'
	import CardSubtitle from 'sveltestrap/src/CardSubtitle.svelte'
	import CardText from 'sveltestrap/src/CardText.svelte'
	import Col from 'sveltestrap/src/Col.svelte'
	import Container from 'sveltestrap/src/Container.svelte'
    import Row from 'sveltestrap/src/Row.svelte'
    
    export let title: string;
    export let desc: string;
    export let url: string;
    export let imgUrl: string;
</script>

<Card class="mb-s">
	<CardHeader>
		<CardTitle class="row align-items-center">
			<strong><a class="black" href={url}>{title}</a></strong>
		</CardTitle>
	</CardHeader>
	<CardBody>
		<Row>
			<Col xs="1" class="pr-0 mr-0">
				<img
					alt={title + ' logo'}
					src={imgUrl} />
			</Col>
			<Col xs="11">
				<CardText>
					{desc}
				</CardText>
			</Col>
		</Row>
		<CardSubtitle class="float-right">
			<a href={url}>Go to website</a>
		</CardSubtitle>
	</CardBody>
</Card>
