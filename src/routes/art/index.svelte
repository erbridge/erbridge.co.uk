<script lang="ts">
  import CategoryIndex from "../../components/CategoryIndex.svelte";

  const pages = [
    {
      title: "seed dispersal",
      slug: "art/seed-dispersal",
      summary: "A walk through Project Gutenberg, one paragraph at a time.",
    },
  ].reverse();
</script>

<CategoryIndex
  title="art"
  description="What even is art? These are the things that serve no purpose other than being interesting to create. Hopefully, they’re also interesting to interact with."
  {pages}
/>
