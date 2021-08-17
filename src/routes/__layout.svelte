<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<Header />
	<slot />
</main>

<style>
	*,
	::before,
	::after {
		box-sizing: border-box;
		transform-style: preserve-3d;
	}
	main {
		min-height: 100vh;
		max-height: 200vh;
		overflow: hidden;
	}
</style>
