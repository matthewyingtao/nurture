<script>
	export let isWhite = true;
</script>

<header id="header">
	<h3><a href=".">Nurture.</a></h3>
	<nav class:white={isWhite}>
		<a href=".">wish</a>
		<a href="unfold">unfold</a>
		<a href="sky">look at the sky</a>
		<a href="blossom">blossom</a>
		<a href="wind">wind</a>
		<a href="flicker">flicker</a>
	</nav>
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 1rem 1rem;
		position: relative;
		z-index: 999;
	}
	header a {
		color: inherit;
	}
	h3 {
		margin: 0;
		font-weight: 300;
		font-size: 1.5em;
	}
	nav {
		list-style: none;
		display: flex;
		margin: 0;
	}
	nav a {
		color: inherit;
		text-decoration: none;
		padding: 0.3rem 0.5rem;
		border-top: solid 1px;
		border-bottom: solid 1px;
		transition: color 250ms ease-out;
		cursor: pointer;
		position: relative;
	}
	nav a:hover {
		color: black;
	}
	nav a::after {
		content: '';
		position: absolute;
		bottom: 0;
		left: 0;
		height: 0%;
		width: 100%;
		background-color: white;
		z-index: -1;
		transition: height 250ms ease-out;
	}
	nav a:hover::after {
		height: 100%;
	}
	nav a:nth-child(2n) {
		border-left: 1px solid;
		border-right: 1px solid;
	}
	nav a:first-child {
		border-left: 1px solid;
		border-top-left-radius: 0.25rem;
		border-bottom-left-radius: 0.25rem;
	}
	nav a:last-child {
		border-right: 1px solid;
		border-top-right-radius: 0.25rem;
		border-bottom-right-radius: 0.25rem;
	}
</style>
