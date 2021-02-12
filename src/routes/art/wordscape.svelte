<script>
  import wordscape from "images/art/wordscape.jpg";
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

  <div class="main-background-image">
    <img role="presentation" src={wordscape} alt="" />
    <div />
  </div>

  <p>
    Download it <a rel="external" href="https://erbridge.itch.io/wordscape"
      >here</a
    >.
  </p>
</Layout>

<style>
  .main-background-image {
    display: none;
  }

  .main-background-image {
    width: 100%;
    max-height: 80vh;
    position: absolute;
    left: 0;
    z-index: -1;
    opacity: 0.1;
    overflow: hidden;
  }

  .main-background-image img {
    width: 100%;
  }

  .main-background-image div {
    width: 100%;
    position: absolute;
    bottom: 0;
    top: 0;
    box-shadow: 0 0 15vw 15vw rgb(var(--background-colour)) inset;
  }

  @media (min-width: 700px) {
    .main-background-image {
      display: block;
    }
  }
</style>
