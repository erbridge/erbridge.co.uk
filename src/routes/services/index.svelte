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
  title="services"
  description="I’ve done a lot of work on web services. This is where most of my “real” releases have been."
  {pages}
/>
