<script>
import Nav from '../../components/Nav.svelte';	
</script>

<style>

	.blog_details{
		margin: 30px;
		background-image: url('../../static/placeholder.jpg');
	}

</style>

<svelte:head>
	<title>Blog</title>
</svelte:head>


<Nav />

<section class="blog_details">

	<h1>Random</h1>

	<h2>Random text random</h2>

	<div class="blog_info">

		<p class="author">Atif</p>

		<p class="date">6/29/2016</p>

		<p class="subject">Computer</p>

	</div>
</section>