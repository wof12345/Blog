<script>
import Blogarticle from '../../components/Blogarticle.svelte';
import Blogpicture from '../../components/Blogpicture.svelte';
import Blogpagedetails from '../../components/Blogpagedetails.svelte';
import { getDate } from '../../components/Date.svelte';

let present = getDate();

let article1,article2,article3;

 article1=article2=article3='Lorem ipsum, dolor sit amet consectetur adipisicing elit. Pariatur, in quasi soluta neque sed, perspiciatis quidem est fuga consequatur aspernatur adipisci et alias voluptates? Adipisci dolorem autem dignissimos ipsa sit.'

let items = {
	articles:[article1,article2,article3],
	pictures:[0,1,2],
}

let fontsize = [17,14,16];
let picturesize = [200,300,400];

</script>

<style>

	.blog_items{
		 max-width: 600px;
		 margin: 10px auto;
		 padding: 20px;
	}

</style>

<svelte:head>
	<title>Blog</title>
</svelte:head>


<Blogpagedetails
title = {'Computer viruses eats away your computer!'}
subject = {'Computer viruses'}
short_detail = {'Computer viruses are a very common in this computer dependent world.'}
author = {'Atif'}
date = {present}
/>

<section class="blog_items">

	{#each items.articles as articles, idx}

	<Blogarticle {fontsize}{idx}{articles}/>

	{/each}

	{#each items.pictures as pictures, idx}

	<Blogpicture {picturesize}{pictures}/>

	{/each}

	{#each items.articles as articles, idx}

	<Blogarticle {fontsize}{idx}{articles}/>

	{/each}





</section>