<header id="header">
	<h3><a href=".">Nurture.</a></h3>
	<nav>
		<a href="/">wish</a>
		<a href="/unfold">unfold</a>
		<a href="/sky">look at the sky</a>
		<a href="/blossom">blossom</a>
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
		border: solid 1px;
	}
	nav a:first-child {
		border-right: none;
		border-top-left-radius: 0.25rem;
		border-bottom-left-radius: 0.25rem;
	}
	nav a:last-child {
		border-left: none;
		border-top-right-radius: 0.25rem;
		border-bottom-right-radius: 0.25rem;
	}
</style>
