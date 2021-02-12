<script>
  import forestWalk from "images/art/forest-walk.jpg";
  import Layout from "../../layouts/art.svelte";
</script>

<Layout title="Forest Walk" description="Walk through an endless forest.">
  <div slot="description">
    <div class="description-background-image">
      <img role="presentation" src={forestWalk} alt="" />
      <div />
    </div>

    <p>A slow game made by:</p>
    <ul>
      <li>
        <a rel="external" href="https://twitter.com/autotwitch">David Fenn</a> (audio)
      </li>
      <li>
        <a rel="external" href="https://twitter.com/Maibbit">Maike Vierkant</a> (illustration)
      </li>
      <li>erbridge (everything else)</li>
    </ul>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/forest-walk">here</a
      >.
    </p>
  </div>

  <div class="main-background-image">
    <img role="presentation" src={forestWalk} alt="" />
    <div />
  </div>

  <pre>walk through an endless forest,
taking in the sights and sounds.
stop, think, look around.
you never know what could be found.</pre>

  <p>
    Download it <a rel="external" href="https://erbridge.itch.io/forest-walk"
      >here</a
    >.
  </p>
</Layout>

<style>
  ul {
    list-style: none;
    padding-left: 0;
    color: rgba(var(--text-colour), 0.8);
  }

  .main-background-image {
    display: none;
  }

  .description-background-image {
    margin-top: -4em;
  }

  .description-background-image,
  .main-background-image {
    width: 100%;
    max-height: 80vh;
    position: absolute;
    left: 0;
    z-index: -1;
    opacity: 0.1;
    overflow: hidden;
  }

  .description-background-image img,
  .main-background-image img {
    width: 100%;
  }

  .description-background-image div,
  .main-background-image div {
    width: 100%;
    position: absolute;
    bottom: 0;
    top: 0;
    box-shadow: 0 0 15vw 15vw rgb(var(--background-colour)) inset;
  }

  pre {
    font-family: var(--body-font-family);
  }

  @media (min-width: 700px) {
    .description-background-image {
      display: none;
    }

    .main-background-image {
      display: block;
    }
  }
</style>
