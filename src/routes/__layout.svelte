<nav class="nav">
	<a href="/">Home</a>
	<a href="/Über">Über</a>
	<a href="/projects">Projekte</a>
</nav>

<slot />

<style lang="scss">
	@import url('https://fonts.googleapis.com/css2?family=Abril+Fatface&display=swap');
	.nav {
		background: rgb(255, 255, 255);
		background: linear-gradient(
			0deg,
			rgba(255, 255, 255, 1) 0%,
			rgba(230, 165, 84, 1) 100%,
			rgba(255, 255, 255, 1) 100%
		);
		height: 4rem;
		display: flex;
		justify-content: space-around;
		align-items: center;

		& a {
			font-weight: 200;
			font-family: Abril Faface;
			font-size: 1.5rem;
			color: black;
			text-decoration: none;
			border-radius: 50%;
		}

		& a:hover {
			background-color: salmon;
		}
	}
</style>
