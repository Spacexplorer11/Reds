<script>
	let { children } = $props();
</script>

<div id="game-background">
	{@render children()}
</div>

<style>
	#game-background {
		@media (prefers-color-scheme: dark) {
			background-image: url("/images/dark-game-bg.webp");
		}
		@media (prefers-color-scheme: light) {
			background-image: url("/images/light-game-bg.webp");
		}
		background-size: cover;
		min-height: 100vh;
		display: flex;
		flex-direction: column;
	}
</style>
