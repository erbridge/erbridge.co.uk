<script>
  import Layout from "../../../layouts/play.svelte";
</script>

<Layout
  title="Voice Engine"
  description="A toolkit for building voice controlled stateful systems."
>
  <div slot="description">
    <div>unreleased</div>

    <p>
      A toolkit for building voice controlled stateful systems made at <a
        rel="external"
        href="https://nianticlabs.com/blog/sensibleobject">Sensible Object</a
      >.
    </p>
  </div>

  <p>
    We built Voice Engine as an tool to make it easier for non-developers to
    collaborate on voice controlled games. It was never released.
  </p>
</Layout>

<style>
  [slot="description"] > :first-child {
    margin-top: -1em;
    font-family: var(--heading-font-family);
  }
</style>
