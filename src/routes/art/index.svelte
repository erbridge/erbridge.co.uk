<script lang="ts">
  import forestWalk from "images/art/forest-walk.jpg";
  import wordscape from "images/art/wordscape.jpg";
  import CategoryIndex from "../../components/CategoryIndex.svelte";

  const pages = [
    {
      title: "@BotCommentator",
      slug: "art/botcommentator",
      summary: "A commentator on Twitter bot games.",
    },
    {
      title: "SEED DISPERSAL",
      slug: "art/seed-dispersal",
      summary: "A walk through Project Gutenberg, one paragraph at a time.",
    },
    {
      title: "@elbownoises",
      slug: "art/elbownoises",
      summary: "A noisy Twitter bot.",
    },
    {
      title: "life maker",
      slug: "art/life-maker",
      summary: "Play Conway’s Game of Life in Github’s contributions graph.",
    },
    {
      title: "@wikipaedian",
      slug: "art/wikipaedian",
      summary: "I sail, node to node, across the seas of Wikipedia’s graph.",
    },
    {
      title: "WordScape",
      slug: "art/wordscape",
      summary: "A screensaver-like of crossing words.",
      background: wordscape,
    },
    {
      title: "Forest Walk",
      slug: "art/forest-walk",
      summary: "Walk through an endless forest.",
      background: forestWalk,
    },
  ].reverse();
</script>

<CategoryIndex
  title="art"
  description="What even is art? These are the things that serve no purpose other than being interesting to create. Hopefully, they’re also interesting to interact with."
  {pages}
/>
