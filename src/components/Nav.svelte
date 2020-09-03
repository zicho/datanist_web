<script>
	import Nav from 'sveltestrap/src/Nav.svelte'
	import NavItem from 'sveltestrap/src/NavItem.svelte'
	import NavLink from 'sveltestrap/src/NavLink.svelte'
	import Navbar from 'sveltestrap/src/Navbar.svelte'
	import NavbarToggler from 'sveltestrap/src/NavbarToggler.svelte'
	import NavbarBrand from 'sveltestrap/src/NavbarBrand.svelte'
	import Collapse from 'sveltestrap/src/Collapse.svelte'

	let isOpen = false

	function handleUpdate(event) {
		isOpen = event.detail.isOpen
	}
</script>

<svelte:head>
	<link
		rel="stylesheet"
		href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" />
</svelte:head>

<Navbar color="dark" class='shadow-lg padding-zero' dark fixed='top' expand="md">
	<NavbarBrand class='margin-l-large' href="/">datanist</NavbarBrand>
	<NavbarToggler on:click={() => (isOpen = !isOpen)} />
	<Collapse {isOpen} navbar expand="md" on:update={handleUpdate}>
		<Nav class="ml-auto" navbar>
			<!-- <NavItem>
				<NavLink href="software">Software</NavLink>
			</NavItem> -->
			<NavItem>
				<NavLink href="about">About me</NavLink>
			</NavItem>
			<NavItem class='margin-r-large'>
				<NavLink href="https://github.com/zicho">GitHub</NavLink>
			</NavItem>
		</Nav>
	</Collapse>
</Navbar>