<script>
	export let segment;
	import Nav from '../components/Nav.svelte';
</script>

<style>

</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>