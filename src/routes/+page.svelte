<script lang="ts">
	import { Head } from "@erbridge/website-theme";
</script>

<Head />

<header>
	<p>hi, my name is F</p>

	<h1>where would you like to go?</h1>
</header>

<section>
	<nav>
		<ul>
			<li><a rel="me" href="//blog.erbridge.co.uk/">blog</a></li>
			<li><a rel="me" href="//library.erbridge.co.uk/">library</a></li>
		</ul>
	</nav>
</section>

<style>
	header {
		margin: 25vh 0 10vh;
	}

	header p {
		margin-bottom: 0;
		line-height: 1.2;
		font-family: var(--heading-font-family);
		font-weight: 600;
		font-size: 1em;
		color: rgb(var(--accent-colour));
	}

	header h1 {
		margin-top: 0.2em;
		margin-bottom: 2em;
		margin-left: 0.8em;
	}

	section {
		margin-bottom: 20vh;
		margin-left: 5em;
		font-size: 1.1em;
	}

	nav {
		display: flex;
		align-items: center;
		font-family: var(--heading-font-family);
		font-weight: 600;
		font-size: 1.2em;
	}

	ul {
		display: flex;
		margin: 0;
		padding: 0;
		flex: 1;
		flex-wrap: wrap;
		list-style: none;
	}

	li {
		margin: 2em;
	}

	@media (min-width: 900px) {
		header {
			font-size: 1.2em;
		}

		section {
			font-size: 1.2em;
		}

		nav {
			margin-left: 4em;
		}
	}

	@media (min-width: 1024px) {
		header {
			font-size: 1.4em;
		}

		section {
			font-size: 1.2em;
		}
	}
</style>
