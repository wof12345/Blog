<script>
	import Nav from '../components/Nav.svelte';
	import Blogcard from '../components/Blogcard.svelte';
</script>

<style>

h1{
	padding: 80px 0px;
	text-align: center;
}

.container{
	margin: 20px;
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(20rem, 1fr));
	align-items: center;
	justify-content: center;
	gap: 30px 5px;
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





