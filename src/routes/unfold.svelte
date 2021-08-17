<svelte:head>
	<title>unfold</title>
</svelte:head>

<section>
	<div class="heading">
		<h1 class="title-main">And I watched the water unfold</h1>
		<h1 class="shadow">And I watched the water unfold</h1>
		<h1 class="shadow">And I watched the water unfold</h1>
		<h1 class="shadow">And I watched the water unfold</h1>
		<h1 class="shadow">And I watched the water unfold</h1>
		<h1 class="shadow">And I watched the water unfold</h1>
	</div>
	<p>It's a feeling I want you to know.</p>
</section>

<div class="scene">
	<div class="cube">
		<div class="face front" />
		<div class="face right" />
		<div class="face back" />
		<div class="face left" />
		<div class="face top" />
		<div class="face bottom" />
	</div>
</div>

<style>
	section {
		max-width: 1140px;
		margin: auto;
		padding: 0 1rem;
		position: relative;
	}
	h1 {
		font-size: 5em;
		margin: 0;
	}
	.heading {
		position: relative;
	}
	.title-main {
		z-index: 1;
		position: relative;
	}
	.shadow {
		position: absolute;
		top: 0;
		left: 0;
		animation: hue-rotate 2s ease-in-out infinite alternate;
		color: red;
	}
	.shadow:nth-child(2) {
		color: blue;
		animation-delay: 0.1s;
	}
	@keyframes hue-rotate {
		0% {
			transform: skewX(-15deg);
		}
		100% {
			transform: skewX(15deg);
		}
	}
	.scene {
		position: absolute;
		z-index: -1;
		top: 15%;
		right: 20%;
		width: 250px;
		height: 250px;
		perspective: 500px;
		filter: drop-shadow(0 0 7rem rgba(255, 255, 255, 0.45));
		animation: float 3s ease-in-out alternate infinite;
	}
	.cube {
		width: 100%;
		height: 100%;
		position: relative;
		animation: rotate 5s linear infinite;
		transform-style: preserve-3d;
	}
	@keyframes float {
		from {
			transform: translateY(125px);
		}
		to {
			transform: translateY(0px);
		}
	}

	@keyframes rotate {
		0% {
			transform: rotateY(0deg) rotateX(65deg) rotateZ(-55deg);
		}
		100% {
			transform: rotateY(360deg) rotateX(65deg) rotateZ(-55deg);
		}
	}
	.face {
		background-image: url('water.jpg');
		background-size: cover;
		background-repeat: no-repeat;
		height: 250px;
		width: 250px;
		position: absolute;
	}
	.front {
		transform: rotateY(0deg) translateZ(125px);
	}
	.back {
		transform: rotateY(180deg) translateZ(125px);
	}
	.left {
		transform: rotateY(-90deg) translateZ(125px);
	}
	.right {
		transform: rotateY(90deg) translateZ(125px);
	}
	.top {
		transform: rotateX(90deg) translateZ(125px);
	}
	.bottom {
		transform: rotateX(-90deg) translateZ(125px);
	}
</style>
