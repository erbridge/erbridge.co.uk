<script lang="ts">
  import { Head } from "@erbridge/website-theme";
  import beastsOfBalance from "images/play/beasts-of-balance.jpg";
  import blindfield from "images/play/blindfield.jpg";
  import whenInRome from "images/play/when-in-rome.jpg";
  import PageLinkList from "../../components/PageLinkList.svelte";

  const releasePages = [
    {
      title: "Beasts of Balance Battles",
      slug: "play/sensible-object/beasts-of-balance-battles",
      summary:
        "A competitive expansion to the digital-tabletop-stacking-meets-strategy game.",
      background: beastsOfBalance,
    },
    {
      title: "When in Rome",
      slug: "play/sensible-object/when-in-rome",
      summary: "The Amazon Alexa-enabled travel trivia social board game.",
      background: whenInRome,
    },
    {
      title: "Word Mine",
      slug: "play/sensible-object/word-mine",
      summary: "A word game played on Amazon Alexa.",
    },
  ].reverse();

  const prototypePages = [
    {
      title: "Blindfield",
      slug: "play/prototypes/blindfield",
      summary: "Search for treasure together in a minefield you can’t see.",
      background: blindfield,
    },
  ].reverse();

  const unreleasedPages = [
    {
      title: "Voice Engine",
      slug: "play/sensible-object/voice-engine",
      summary: "A toolkit for building voice controlled stateful systems.",
    },
  ].reverse();
</script>

<Head
  title="play"
  description="I was a game developer in a past life. Here’s the back catalogue of the things I had a hand in creating."
/>

<h1>play</h1>

<p>
  I was a game developer in a past life. Here’s the back catalogue of the things
  I had a hand in creating.
</p>

<h2>releases</h2>

<PageLinkList pages={releasePages} headingLevel={3} />

<h2>prototypes</h2>

<PageLinkList pages={prototypePages} headingLevel={3} />

<h2>unreleased</h2>

<PageLinkList pages={unreleasedPages} headingLevel={3} />
