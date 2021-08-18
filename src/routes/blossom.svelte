<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<Header />
	<section>
		<h2>And we wished each other well</h2>
		<div class="dirt-container">
			<img class="dirt" src="./dirt.jpg" alt="dirt" />
		</div>
		<a href="wind">
			<div class="fire">
				<img class="red" src="/fire-red.png" alt="fire" />
				<img class="orange" src="/fire-orange.png" alt="fire" />
				<img class="yellow" src="/fire-yellow.png" alt="fire" />
			</div>
		</a>
	</section>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
	}
	section {
		display: flex;
		justify-content: center;
		align-items: center;
		position: relative;
		height: 100%;
		width: 100%;
	}
	h2 {
		position: absolute;
		top: 0;
		font-size: 4em;
		font-weight: 200;
	}
	.fire {
		position: relative;
		z-index: 2;
	}
	.fire img {
		height: 25em;
	}
	.red {
		filter: drop-shadow(0 -5em 6em rgba(255, 166, 0, 0.6));
		animation: wave 3s ease-in-out alternate infinite;
	}
	.orange {
		filter: drop-shadow(0 -4em 4em rgba(255, 166, 0, 0.6));
		animation: wave 2.5s ease-in-out alternate infinite;
		position: absolute;
		top: 0;
		left: 0;
	}
	.yellow {
		filter: drop-shadow(0 -1em 2em rgba(255, 255, 0, 0.6));
		animation: wave 2s alternate ease-in-out infinite;
		position: absolute;
		top: 0;
		left: 0;
	}
	@keyframes wave {
		0% {
			transform: translate(-10px, -10px);
		}
		50% {
			transform: translate(0px, 10px);
		}
		to {
			transform: translate(10px, -10px);
		}
	}
	.dirt {
		transform: perspective(5em) translateY(50%) rotateX(20deg);
		width: 100%;
		height: 100%;
		object-fit: cover;
	}
	.dirt-container {
		background: radial-gradient(circle, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 1) 12%);
		transform: perspective(5em) translateY(50%) rotateX(20deg) scaleX(5);
		position: absolute;
		bottom: 0;
		left: 0;
		width: 100%;
		height: 100%;
		transform-style: preserve-3d;
	}
</style>
