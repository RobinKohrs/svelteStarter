<script>
	let pages = ['Maps', 'Photos', 'Archi', 'Rest'];
</script>

<svelte:head>
	<title>Experimentsk</title>
</svelte:head>

<div class="first-site-container">
	{#each pages as page, i}
		<div
			class="link flex {i % 2 == 0 ? 'justify-start' : 'justify-end'}"
			style={i % 2 == 0 ? 'padding-left: 3rem;' : 'padding-right: 3rem;'}
		>
			<a href="/Über">{page}</a>
		</div>
	{/each}
</div>

<style lang="scss">
	.first-site-container {
		padding: 0;
		position: absolute;
		bottom: 50%;
		left: 50%;
		width: 50vw;
		transform: translateX(-50%) translateY(50%);

		.link {
			font-size: 3rem;
			border-bottom: 1px solid transparent;
		}
		.link:hover {
			border-bottom: 1px solid black;
		}
	}
</style>
