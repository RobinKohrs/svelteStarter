<!-- src/routes/__layout.svelte -->

<nav class="nav">
	<a href="/">Home</a>
	<a href="/Über">Über</a>
	<a href="/projects">Projekte</a>
</nav>

<slot />

<style lang="scss">
	.nav {
		display: flex;
		justify-content: space-around;
	}
</style>
