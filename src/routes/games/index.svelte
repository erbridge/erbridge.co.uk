<script lang="ts">
  import { Head } from "@erbridge/website-theme";
  import beastsOfBalance from "images/games/beasts-of-balance.jpg";
  import blindfield from "images/games/blindfield.jpg";
  import whenInRome from "images/games/when-in-rome.jpg";
  import PageLinkList from "../../components/PageLinkList.svelte";

  const releasePages = [
    {
      title: "Beasts of Balance Battles",
      slug: "games/sensible-object/beasts-of-balance-battles",
      summary:
        "A competitive expansion to the digital-tabletop-stacking-meets-strategy game.",
      background: beastsOfBalance,
    },
    {
      title: "When in Rome",
      slug: "games/sensible-object/when-in-rome",
      summary: "The Amazon Alexa-enabled travel trivia social board game.",
      background: whenInRome,
    },
  ].reverse();

  const prototypePages = [
    {
      title: "Blindfield",
      slug: "games/prototypes/blindfield",
      summary: "Search for treasure together in a minefield you can’t see.",
      background: blindfield,
    },
  ].reverse();

  const unreleasedPages = [
    {
      title: "Voice Engine",
      slug: "games/sensible-object/voice-engine",
      summary: "A toolkit for building voice controlled stateful systems.",
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

<h2>releases</h2>

<PageLinkList pages={releasePages} headingLevel={3} />

<h2>prototypes</h2>

<PageLinkList pages={prototypePages} headingLevel={3} />

<h2>unreleased</h2>

<PageLinkList pages={unreleasedPages} headingLevel={3} />
