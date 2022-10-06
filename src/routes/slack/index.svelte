<script lang="ts">
  import CategoryIndex from "../../components/CategoryIndex.svelte";

  const pages = [
    {
      title: "WordScape",
      slug: "art/wordscape",
      summary: "A screensaver-like of crossing words.",
    },
  ].reverse();
</script>

<CategoryIndex
  title="slack"
  description="I like automating things, especially if those things are cultural shifts. Slack bots are a prime example."
  {pages}
/>
