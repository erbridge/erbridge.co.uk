<script lang="ts">
  import { Head } from "@erbridge/website-theme";
  import blindfield from "images/games/blindfield.jpg";
  import PageLinkList from "../../components/PageLinkList.svelte";

  const prototypePages = [
    {
      title: "Blindfield",
      slug: "games/prototypes/blindfield",
      summary: "Search for treasure together in a minefield you can’t see.",
      background: blindfield,
    },
  ].reverse();
</script>

<Head
  title="games"
  description="I was a game developer in a past life. Here’s the back catalogue of everything I ever had a hand in creating."
/>

<h1>games</h1>

<p>
  I was a game developer in a past life. Here’s the back catalogue of everything
  I ever had a hand in creating.
</p>

<h2>prototypes</h2>

<PageLinkList pages={prototypePages} headingLevel={3} />
