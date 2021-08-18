<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<Header />
	<section>
		<a href="/">
			<img class="shoe" src="/shoe.png" alt="shoe" />
		</a>
	</section>
</main>

<style>
	main {
		background: url('/posters.jpg');
		color: black;
		display: flex;
		flex-direction: column;
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
		animation: shoe 1.5s ease-in-out infinite alternate;
	}
	@keyframes shoe {
		0% {
			transform: rotateZ(35deg);
			filter: hue-rotate(0deg);
		}
		100% {
			transform: rotateZ(0deg);
			filter: hue-rotate(360deg);
		}
	}
</style>
