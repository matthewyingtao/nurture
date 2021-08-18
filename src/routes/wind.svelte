<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<Header />
	<a href="/">
		<img class="train" src="/snow.jpg" alt="train" />
	</a>
</main>

<style>
	main {
		background-image: url('/countryside.jpg');
	}
	.train {
		mask-image: url('/train.svg');
		-webkit-mask-image: url('/train.svg');
		width: 100%;
		max-height: 80vh;
		object-fit: cover;
		mask-repeat: no-repeat;
		-webkit-mask-repeat: no-repeat;
		mask-size: 35em;
		-webkit-mask-size: 35em;
		animation: slide 5s linear infinite;
	}
	@keyframes slide {
		from {
			-webkit-mask-position: calc(100% + 35em) center;
			mask-position: calc(100% + 35em) center;
		}
		to {
			-webkit-mask-position: -100% center;
			mask-position: -100% center;
		}
	}
</style>
