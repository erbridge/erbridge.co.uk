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
  title="other"
  description="Some things defy categorization. Others are in categories of one. These are those."
  {pages}
/>
