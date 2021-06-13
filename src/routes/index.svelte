<script>
	import Nav from '../components/Nav.svelte';
	import Blogcard from '../components/Blogcard.svelte';
</script>

<style>
:root{
	--cover_value:40%;
}

h1{
	padding: 80px 0px;
	text-align: center;
}

.container{
	margin: 20px;
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(var(--cover_value), 1fr));
	align-items: center;
	justify-content: center;
	gap: 30px 5px;
}

@media screen and (max-width: 883px) {
	:root{
	--cover_value:100%;
}
}

@media screen and (max-width: 700px) {
	:root{
	--cover_value:100%;
}
}

@media screen and (max-width: 345px) {
	.container{
		margin: 0;
	}
}

</style>


<Nav />

<h1>
	Latest contents
</h1>

<div class="container">

	<Blogcard />

	<Blogcard />

	<Blogcard />

	<Blogcard />

	<Blogcard />

</div>





