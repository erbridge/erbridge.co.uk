<script lang="ts">
	import { ThemeToggle } from "@erbridge/website-theme";
	import "@erbridge/website-theme/stylesheets/global.css";
	import "normalize.css";
</script>

<svelte:head>
	<meta name="theme-color" content="#000000" />

	<style>
		:root {
			--background-colour: 0, 0, 0;
			--text-colour: 255, 255, 255;
			--accent-colour: 127, 127, 127;
			--secondary-accent-colour: 127, 127, 127;
		}

		:root.theme--light {
			--background-colour: 255, 255, 255;
			--text-colour: 0, 0, 0;
			--accent-colour: 127, 127, 127;
			--secondary-accent-colour: 127, 127, 127;
		}

		@media (prefers-color-scheme: light) {
			:root:not(.theme--dark) {
				--background-colour: 255, 255, 255;
				--text-colour: 0, 0, 0;
				--accent-colour: 127, 127, 127;
				--secondary-accent-colour: 127, 127, 127;
			}
		}
	</style>
</svelte:head>

<header>
	<ThemeToggle />
</header>

<main>
	<slot />
</main>

<style>
	header,
	main {
		max-width: 58rem;
		width: 100%;
	}

	header {
		margin: 1rem auto;
		padding: 0 1rem;
		min-height: 2em;
		font-size: 1.2rem;
		display: flex;
		align-items: center;
		justify-content: flex-end;
	}

	main {
		margin: 0 auto;
		padding: 1rem;
		min-height: 0;
		flex-grow: 1;
	}
</style>
