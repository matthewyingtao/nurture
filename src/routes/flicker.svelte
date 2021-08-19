<script>
	import Header from '../components/Header.svelte';
</script>

<main>
	<img class="bg" src="/posters.jpg" alt="posters" />
	<Header />
	<section>
		<a href="/mirror">
			<img class="shoe" src="/shoe.png" alt="shoe" />
		</a>
		<h2>"I'm just trying to find what's important."</h2>
	</section>
</main>

<style>
	main {
		color: black;
		display: flex;
		flex-direction: column;
		overflow: hidden;
	}
	.bg {
		position: absolute;
		z-index: -1;
		top: 0;
		left: 0;
		height: 100%;
		width: 100%;
		object-fit: cover;
		animation: rainbow 7s steps(10) infinite reverse;
	}
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100%;
	}
	h2 {
		font-size: 4em;
		width: 500px;
		text-align: right;
		animation: fuckedup 6s infinite steps(50);
	}
	@keyframes fuckedup {
		2% {
			font-weight: 200;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		4% {
			font-weight: 600;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
			text-align: center;
		}
		6% {
			font-weight: 400;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
			letter-spacing: 3px;
		}
		8% {
			font-weight: 600;
			font-style: normal;
			text-decoration: underline;
			text-transform: none;
		}
		10% {
			font-weight: 100;
			font-style: normal;
			text-decoration: underline;
			text-transform: capitalize;
			text-align: left;
		}
		12% {
			font-weight: 700;
			font-style: normal;
			text-decoration: underline;
			text-transform: none;
		}
		14% {
			font-weight: 500;
			font-style: normal;
			text-decoration: none;
			letter-spacing: -5px;
			text-transform: lowercase;
			text-align: justify;
		}
		16% {
			font-weight: 100;
			font-style: normal;
			text-decoration: underline;
			text-transform: none;
		}
		18% {
			font-weight: 400;
			font-style: italic;
			text-decoration: line-through;
			text-transform: uppercase;
			text-align: end;
		}
		20% {
			font-weight: 500;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		22% {
			font-weight: 100;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		24% {
			font-weight: 700;
			font-style: normal;
			text-decoration: underline;
			text-transform: lowercase;
		}
		26% {
			font-weight: 500;
			font-style: normal;
			text-decoration: underline;
			text-transform: none;
		}
		28% {
			font-weight: 500;
			font-style: normal;
			text-decoration: underline;
			text-align: left;
			text-transform: none;
		}
		30% {
			font-weight: 100;
			font-style: normal;
			text-decoration: none;
			text-transform: lowercase;
		}
		32% {
			font-weight: 700;
			font-style: normal;
			text-decoration: none;
			text-transform: capitalize;
		}
		34% {
			font-weight: 300;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		36% {
			font-weight: 600;
			font-style: normal;
			text-decoration: none;
			text-transform: capitalize;
		}
		38% {
			font-weight: 100;
			font-style: italic;
			text-decoration: none;
			text-transform: lowercase;
		}
		40% {
			font-weight: 100;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		42% {
			font-weight: 400;
			font-style: normal;
			text-decoration: none;
			text-transform: lowercase;
		}
		44% {
			font-weight: 400;
			font-style: normal;
			text-decoration: line-through;
			text-transform: none;
		}
		46% {
			font-weight: 700;
			font-style: italic;
			text-decoration: none;
			text-transform: lowercase;
		}
		48% {
			font-weight: 300;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		50% {
			font-weight: 600;
			font-style: normal;
			text-decoration: none;
			text-align: justify;
			text-transform: none;
		}
		52% {
			font-weight: 500;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		54% {
			font-weight: 300;
			font-style: normal;
			text-decoration: underline;
			text-transform: lowercase;
		}
		56% {
			font-weight: 700;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		58% {
			font-weight: 500;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		60% {
			font-weight: 200;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		62% {
			font-weight: 400;
			font-style: italic;
			text-decoration: none;
			text-transform: lowercase;
		}
		64% {
			font-weight: 100;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		66% {
			font-weight: 400;
			text-align: right;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		68% {
			font-weight: 700;
			font-style: normal;
			text-decoration: line-through;
			text-transform: none;
		}
		70% {
			font-weight: 400;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		72% {
			font-weight: 200;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		74% {
			font-weight: 100;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		76% {
			font-weight: 600;
			font-style: normal;
			text-decoration: underline;
			text-align: left;
			text-transform: none;
		}
		78% {
			font-weight: 500;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		80% {
			font-weight: 200;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		82% {
			font-weight: 100;
			font-style: normal;
			text-decoration: none;
			text-transform: lowercase;
		}
		84% {
			font-weight: 200;
			font-style: italic;
			text-decoration: none;
			text-transform: none;
		}
		86% {
			font-weight: 100;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		88% {
			font-weight: 700;
			font-style: normal;
			text-decoration: underline;
			text-transform: capitalize;
		}
		90% {
			font-weight: 400;
			font-style: italic;
			text-decoration: none;
			text-transform: uppercase;
		}
		92% {
			font-weight: 500;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		94% {
			font-weight: 500;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		96% {
			font-weight: 400;
			font-style: normal;
			text-decoration: none;
			text-transform: none;
		}
		98% {
			font-weight: 300;
			font-style: normal;
			text-decoration: underline;
			text-transform: none;
		}
	}
	.shoe {
		height: 15em;
		transform-origin: bottom right;
		animation: rainbow 1s infinite, float 2s steps(20) infinite;
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
	@keyframes float {
		0% {
			transform: translateY(125px) rotateZ(60deg);
			filter: drop-shadow(0 calc(20em - 250px) 2rem rgba(0, 0, 0, 0.6));
		}
		20% {
			filter: drop-shadow(0 20em 6rem rgba(0, 0, 0, 0.3));
			transform: translateY(150px) rotateX(15deg);
		}
		40% {
			filter: drop-shadow(0 20em 6rem rgba(0, 0, 0, 0.3));
			transform: translateY(150px) skewY(25deg);
		}
		60% {
			filter: drop-shadow(0 20em 3.2rem rgba(0, 0, 0, 0.3));
			transform: translateY(0px) skewX(10deg) skewY(5deg);
		}
		80% {
			filter: drop-shadow(0 20em 3rem rgba(0, 0, 0, 0.3));
			transform: translateY(10px) skewX(16deg) skewY(10deg);
		}
		100% {
			filter: drop-shadow(0 20em 1rem rgba(0, 0, 0, 0.3));
			transform: translateY(-150px);
		}
	}
</style>
