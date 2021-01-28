<script lang="ts">
  import CategoryIndex from "../../components/CategoryIndex.svelte";

  const pages = [
    {
      title: "USER ERROR",
      slug: "writing/user-error",
      extract:
        "I looked at the pair of figures lying motionless in the dark, damp room. Water dripped from a pipe nearby and the smell of blood filled my nostrils",
    },
    {
      title: "The Groaning Worm (Part II)",
      slug: "writing/the-groaning-worm-part-ii",
      extract:
        "The magicians and phonetic monsters / Have their ministries; they waste alongside the terror, / Never tasting it; their exhortations are faltering",
    },
    {
      title: "and so the wheel turns",
      slug: "writing/and-so-the-wheel-turns",
      extract:
        "And so the wheel turns. / The bracken breaks beneath my feet, / As these words roll over my tongue",
    },
    {
      title: "REC",
      slug: "writing/rec",
      summary:
        "A cameraman, interrupted from filming a new skate video by a streak of fire in the sky, documents his final hours.",
    },
    {
      title: "under the light of a dying star",
      slug: "writing/under-the-light-of-a-dying-star",
      extract:
        "Under the light of a dying star, Aaron McBarnes sits in front of his television. The show he’s watching is hilarious, sending him into fits of laughter, reminding him of his grandmother",
    },
    {
      title: "for your safety",
      slug: "writing/for-your-safety",
      extract:
        "Thirty seven thousand feet. / THE VOMIT-METER, / says the mauve paper in the seat in front",
    },
    {
      title: "the tree",
      slug: "writing/the-tree",
      extract:
        "The tree beckons. / Its twisted limbs reaching out, / calling, / summoning",
    },
    {
      title: "face",
      slug: "writing/face",
      extract: "I wear it. / The face of happiness, / while it boils beneath",
    },
    {
      title: "sessions",
      slug: "writing/sessions",
      extract:
        "Thoughts and feelings, / Overwhelming. passions and / Truths. multiple and deafening",
    },
    {
      title: "dancers",
      slug: "writing/dancers",
      extract:
        "Cold skin, warm heart. / On a pedestal, exposed. Seen. / Curves and motion examined",
    },
  ].reverse();
</script>

<CategoryIndex
  title="writing"
  description="Sometimes I write. I’m particularly fond of poetry, but there are some other writing forms here. Some are experiments, others are reflections on emotions or events. Some are very old and probably not very good. Some are new and also not very good."
  {pages}
/>
