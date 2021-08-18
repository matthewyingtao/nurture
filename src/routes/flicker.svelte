<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<img class="bg" src="/posters.jpg" alt="posters" />
	<Header />
	<section>
		<a href="/">
			<img class="shoe" src="/shoe.png" alt="shoe" />
		</a>
	</section>
</main>

<style>
	main {
		color: black;
		display: flex;
		flex-direction: column;
	}
	.bg {
		position: absolute;
		z-index: -1;
		top: 0;
		left: 0;
		height: 100%;
		width: 100%;
		animation: rainbow 7s infinite reverse;
	}
	section {
		display: flex;
		justify-content: center;
		align-items: center;
		height: 100%;
	}
	.shoe {
		height: 15em;
		transform-origin: bottom right;
		animation: rainbow 1s steps(36) infinite;
	}
	@keyframes rainbow {
		from {
			-webkit-filter: hue-rotate(0deg);
			filter: hue-rotate(0deg);
		}
		to {
			-webkit-filter: hue-rotate(360deg);
			filter: hue-rotate(360deg);
		}
	}
</style>
