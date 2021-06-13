<script>
	export let segment;
	import Nav from '../components/Nav.svelte';
</script>

<style>
main>*{
	font-family: 'Montserrat', sans-serif;
}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>