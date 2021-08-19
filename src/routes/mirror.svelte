<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<img class="bg" src="/forest.jpg" alt="forest" />
	<Header />
	<section>
		<div class="text">
			<h2>"The best sort of inner voice" she began,</h2>
			<h2>"speaks to us in a gentle kind, and unhurried way."</h2>
		</div>
		<div class="flowers">
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="flower" src="/flower.svg" alt="flower" />
			<img class="fairy" src="/fairy.svg" alt="fairy" />
		</div>
	</section>
</main>

<style>
	.bg {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		image-rendering: pixelated;
		object-fit: cover;
	}
	section {
		height: 80vh;
	}
	.text {
		position: absolute;
		top: 0;
		z-index: 1;
		right: 0;
		margin-left: auto;
	}
	h2 {
		font-weight: 200;
		font-size: 2em;
		text-align: right;
		background: black;
		padding: 0.2em;
		width: max-content;
		margin-left: auto;
	}
	.flower {
		position: absolute;
		height: 150px;
		animation: spin 5s linear infinite;
	}
	.flower:nth-child(1) {
		bottom: 14%;
		left: 78%;
		animation-delay: 347ms;
	}
	.flower:nth-child(2) {
		bottom: 69%;
		left: 68%;
		animation-delay: 35ms;
	}
	.flower:nth-child(3) {
		bottom: 90%;
		left: 98%;
		animation-delay: 559ms;
	}
	.flower:nth-child(4) {
		bottom: 37%;
		left: 84%;
		animation-delay: 792ms;
	}
	.flower:nth-child(5) {
		bottom: 73%;
		left: 1%;
		animation-delay: 738ms;
	}
	.flower:nth-child(6) {
		bottom: 75%;
		left: 7%;
		animation-delay: 86ms;
	}
	.flower:nth-child(7) {
		bottom: 1%;
		left: 76%;
		animation-delay: 667ms;
	}
	.flower:nth-child(8) {
		bottom: 32%;
		left: 18%;
		animation-delay: 858ms;
	}
	.flower:nth-child(9) {
		bottom: 54%;
		left: 50%;
		animation-delay: 995ms;
	}
	.flower:nth-child(10) {
		bottom: 4%;
		left: 54%;
		animation-delay: 200ms;
	}
	@keyframes spin {
		from {
			transform: rotateY(0deg);
		}
		to {
			transform: rotateY(360deg);
		}
	}
	.fairy {
		position: absolute;
		width: 500px;
		top: 0;
		left: 0;
		transform: translate(50%, 50%);
	}
</style>
