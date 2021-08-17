<header>
	<h3><a href=".">Nurture.</a></h3>
	<nav>
		<a href="wish">wish</a>
		<a href="unfold">unfold</a>
		<a href="wish">wish</a>
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
		color: white;
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
		color: white;
		text-decoration: none;
		padding: 0.3rem 0.5rem;
		border: white solid 1px;
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
