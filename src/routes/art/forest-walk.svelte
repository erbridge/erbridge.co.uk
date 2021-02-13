<script>
  import forestWalk from "images/art/forest-walk.jpg";
  import PageBackgroundImage from "../../components/PageBackgroundImage.svelte";
  import Layout from "../../layouts/art.svelte";
</script>

<Layout title="Forest Walk" description="Walk through an endless forest.">
  <div slot="description">
    <p>A slow game made by:</p>
    <ul>
      <li>
        <a rel="external" href="https://twitter.com/autotwitch">David Fenn</a> (audio)
      </li>
      <li>
        <a rel="external" href="https://twitter.com/Maibbit">Maike Vierkant</a> (illustration)
      </li>
      <li>me (everything else)</li>
    </ul>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/forest-walk">here</a
      >.
    </p>
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

  <PageBackgroundImage src={forestWalk} />
</Layout>

<style>
  ul {
    list-style: none;
    padding-left: 0;
    color: rgba(var(--text-colour), 0.8);
  }

  pre {
    font-family: var(--body-font-family);
  }
</style>
