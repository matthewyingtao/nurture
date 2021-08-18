<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<Header />
	<a href="/flicker">
		<img class="train" src="/snow.jpg" alt="train" />
	</a>
	<section>
		<h2>Or I'll dream of you</h2>
	</section>
</main>

<style>
	main {
		background-image: url('/countryside.jpg');
		background-repeat: no-repeat;
		display: flex;
		flex-direction: column;
	}
	section {
		position: absolute;
		margin: auto;
		top: 0;
		left: 0;
		height: 100%;
		width: 100%;
		display: flex;
		justify-content: center;
		align-items: center;
		pointer-events: none;
	}
	h2 {
		font-weight: 200;
		font-size: 4em;
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
