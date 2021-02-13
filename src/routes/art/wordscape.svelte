<script>
  import wordscape from "images/art/wordscape.jpg";
  import PageBackgroundImage from "../../components/PageBackgroundImage.svelte";
  import Layout from "../../layouts/art.svelte";
</script>

<Layout title="WordScape" description="A screensaver-like of crossing words.">
  <div slot="description">
    <p>
      A screensaver-like of crossing words, built for <a
        rel="external"
        href="http://itch.io/jam/screensaverjam">#screensaverjam</a
      >.
    </p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/wordscape">here</a
      >.
    </p>
  </div>

  <PageBackgroundImage src={wordscape} type="main" />

  <p>
    Download it <a rel="external" href="https://erbridge.itch.io/wordscape"
      >here</a
    >.
  </p>
</Layout>
