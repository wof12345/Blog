<script>
import Blogarticle from '../../components/Blogarticle.svelte';
import Blogpicture from '../../components/Blogpicture.svelte';

let items = {
	articles:[0,1,2],
	pictures:[0,1,2],
}

let fontsize = [13,14,16];
let picturesize = [200,300,400];

</script>

<style>

	.blog_details{
		margin: 30px;
		background-image: url('/placeholder.jpg');
		background-size: 100%;
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
		background-position: center;
		padding: 70px;
	}

	.blog_details>*{
		color: white;
	}	

	.blog_items{
		 max-width: 600px;
		 margin: 10px auto;
		 padding: 20px;
	}

</style>

<svelte:head>
	<title>Blog</title>
</svelte:head>


<section class="blog_details">

	<h1>Random</h1>

	<h2>Random text random</h2>

	<div class="blog_info">

		<p class="author">Atif</p>

		<p class="date">6/29/2016</p>

		<p class="subject">Computer</p>

	</div>
</section>

<section class="blog_items">

	{#each items.articles as articles, idx}

	<Blogarticle {fontsize}{articles}/>

	{/each}

	{#each items.pictures as pictures, idx}

	<Blogpicture {picturesize}{pictures}/>

	{/each}

	{#each items.articles as articles, idx}

	<Blogarticle {fontsize}{articles}/>

	{/each}





</section>