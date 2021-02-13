<script>
  import memoryLeak from "images/art/memory-leak.jpg";
  import PageBackgroundImage from "../../components/PageBackgroundImage.svelte";
  import Layout from "../../layouts/art.svelte";
</script>

<Layout title="Memory Leak" description="A bad joke.">
  <div slot="description">
    <p>A “game” made for Nordic Game Jam 2016. The theme was “Leak!”</p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/memory-leak">here</a
      >.
    </p>
  </div>

  <p>Stop the memory from leaking by clicking on the escaping memory chips.</p>

  <p>I think that's right...</p>

  <p>
    Play with it <a rel="external" href="https://erbridge.itch.io/memory-leak"
      >here</a
    >.
  </p>

  <PageBackgroundImage src={memoryLeak} />
</Layout>
