<script>
	import Blogcard from '../components/Blogcard.svelte';
	import { getDate } from '../components/Date.svelte';

	let present = getDate();

	let articles =[0,1,2];
</script>

<style>
:root{
	--cover_value:40%;
	--cover_value1:300px;
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
	gap: 30px 20px;
}

/* .container1{
	margin: 20px;
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(var(--cover_value1), 1fr));
	align-items: center;
	justify-content: center;
	gap: 30px 20px;
} */

@media screen and (max-width: 883px) {
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


<h1>
	Latest contents
</h1>

<section class="container">

	{#each articles as articles }
		<Blogcard 
		title = {'Computer viruses eats away your computer!'}
		subject = {'Computer viruses'}
		short_detail = {'Computer viruses are a very common in this computer dependent world.'}
		author = {'Atif'}
		date = {present}
		/>
	{/each}


</section>


<h1>
	Other contents
</h1>

<section class="container">

	{#each articles as articles }
		<Blogcard 
		title = {'Computer viruses eats away your computer!'}
		subject = {'Computer viruses'}
		short_detail = {'Computer viruses are a very common in this computer dependent world.'}
		author = {'Atif'}
		date = {present}
		/>
	{/each}


</section>





