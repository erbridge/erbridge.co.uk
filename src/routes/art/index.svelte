<script lang="ts">
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
  ].reverse();
</script>

<CategoryIndex
  title="art"
  description="What even is art? These are the things that serve no purpose other than being interesting to create. Hopefully, they’re also interesting to interact with."
  {pages}
/>
