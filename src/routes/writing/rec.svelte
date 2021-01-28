<script>
  import Layout from "../../layouts/writing.svelte";
</script>

<Layout
  title="REC"
  description="A cameraman, interrupted from filming a new skate video by a streak of fire in the sky, documents his final hours."
  opaqueHeader
>
  <div slot="description">
    <p>
      A cameraman, interrupted from filming a new skate video by a streak of
      fire in the sky, documents his final hours.
    </p>

    <p>
      <a rel="external" href="https://www.impact50film.com/create50/"
        >Impact:50</a
      >
      was a collaborative filmmaking process that selected 50 scripts and combined
      them to create a single film. <span class="mono">REC</span> was my (unselected)
      submission, intended to be split up and dispersed through the larger narrative.
    </p>

    <p><strong>Content warning: existential threat</strong></p>

    <p><small>Please ignore my deadname in the PDF…</small></p>
  </div>

  <div class="pdf">
    <object
      aria-label="The screenplay, REC"
      role="document"
      data="assets/rec.pdf"
      type="application/pdf"
    />

    <p><a role="button" href="assets/rec.pdf">Download the PDF</a></p>
  </div>
</Layout>

<style>
  .mono {
    font-family: var(--monospace-font-family);
  }

  .pdf {
    height: 100%;
    display: flex;
    flex-direction: column;
  }

  object {
    width: 100%;
    min-height: 400px;
    max-height: 90vh;
    flex-grow: 1;
  }
</style>
