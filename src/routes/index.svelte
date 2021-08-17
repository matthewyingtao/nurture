<script>
	import Parallax from 'parallax-js';

	let parallaxInstance;

	const ready = (node) => {
		console.log(node);
		parallaxInstance = new Parallax(node);
	};

	let title = 'get your wish';
</script>

<svelte:head>
	<title>wish</title>
</svelte:head>
<a href="unfold">
	<div use:ready class="wish">
		<div class="img-container" data-depth="1.2">
			<img class="water" src="water.jpg" alt="get your wish" />
			<div class="reflect">
				<img src="water.jpg" alt="get your wish" />
				<div class="reflect-gradient" />
			</div>
		</div>

		<div class="layer" data-depth="0.6">
			<h2>{title}</h2>
		</div>
	</div>
</a>

<style>
	.wish {
		display: flex;
		align-items: center;
		justify-content: center;
		position: relative;
	}
	.img-container {
		width: clamp(300px, 70%, 778px);
		position: relative;
	}
	.img-container img {
		width: 100%;
		height: 100%;
		display: block;
	}
	.img-container::after {
		content: '';
		position: absolute;
		height: 100%;
		width: 100%;
		top: 0;
		left: 0;
		box-shadow: inset 0 4.5em 4em 2.5em black;
		background: radial-gradient(circle, rgba(0, 0, 0, 0) 0%, rgba(0, 0, 0, 0.8) 60%);
	}
	.reflect {
		position: absolute;
		top: 0;
		left: 0;
		transform: perspective(5em) translateY(50%) scaleY(-1) rotateX(20deg);
		z-index: -1;
	}
	.reflect-gradient {
		position: absolute;
		top: 0;
		left: 0;
		height: 100%;
		width: 100%;
		background: radial-gradient(circle, rgba(0, 0, 0, 0.9) 0%, rgba(0, 0, 0, 1) 90%);
		box-shadow: inset 0 -0.5em 7em -1.5em black;
	}
	.wish h2 {
		color: white;
		padding: 0.1em;
		margin-top: 2em;
		font-size: 4em;
		font-weight: 200;
	}
	.layer {
		position: absolute;
		width: 100%;
		height: 100%;
		display: flex !important;
		align-items: center;
		justify-content: center;
	}
</style>
