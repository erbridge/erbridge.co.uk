<script>
  import memoryLeak from "images/art/memory-leak.jpg";
  import Layout from "../../layouts/art.svelte";
</script>

<Layout title="Memory Leak" description="A bad joke.">
  <div slot="description">
    <div class="description-background-image">
      <img role="presentation" src={memoryLeak} alt="" />
      <div />
    </div>

    <p>A “game” made for Nordic Game Jam 2016. The theme was “Leak!”</p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/memory-leak">here</a
      >.
    </p>
  </div>

  <div class="main-background-image">
    <img role="presentation" src={memoryLeak} alt="" />
    <div />
  </div>

  <p>Stop the memory from leaking by clicking on the escaping memory chips.</p>

  <p>I think that's right...</p>

  <p>
    Play with it <a rel="external" href="https://erbridge.itch.io/memory-leak"
      >here</a
    >.
  </p>
</Layout>

<style>
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

  @media (min-width: 700px) {
    .description-background-image {
      display: none;
    }

    .main-background-image {
      display: block;
    }
  }
</style>
