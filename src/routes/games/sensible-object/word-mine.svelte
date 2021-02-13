<script>
  import Layout from "../../../layouts/games.svelte";
</script>

<Layout title="Word Mine" description="A word game played on Amazon Alexa.">
  <div slot="description">
    <div>discontinued</div>

    <p>
      An Amazon Alexa game made at <a
        rel="external"
        href="https://nianticlabs.com/blog/sensibleobject">Sensible Object</a
      >.
    </p>
  </div>

  <p>
    Descend into the Word Mine every day to excavate letters. Find an anagram of
    those letters quickly to release them from the rock, and sell them on the
    surface to upgrade your gear.
  </p>

  <p>No longer available.</p>
</Layout>

<style>
  [slot="description"] > :first-child {
    margin-top: -1em;
    font-family: var(--heading-font-family);
  }
</style>
