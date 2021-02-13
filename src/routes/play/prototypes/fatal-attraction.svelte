<script>
  import fatalAttraction from "images/play/fatal-attraction.jpg";
  import PageBackgroundImage from "../../../components/PageBackgroundImage.svelte";
  import Layout from "../../../layouts/play.svelte";
</script>

<Layout
  title="Fatal Attraction"
  description="Change gravity to avoid crashing."
>
  <div slot="description">
    <div>prototype</div>

    <p>
      Made in 48 hours for <a
        rel="external"
        href="http://ludumdare.com/compo/ludum-dare-32/?action=preview&uid=34508"
        >Ludum Dare 32</a
      >.
    </p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/fatal-attraction">here</a
      >.
    </p>
  </div>

  <p>
    Fatal Attraction is a gravity based arcade game. Rotate your ship and use
    your gun to change the gravity source. Try not to crash into anything.
  </p>

  <p>
    Play it <a rel="external" href="https://erbridge.itch.io/fatal-attraction"
      >here</a
    >.
  </p>

  <PageBackgroundImage src={fatalAttraction} />
</Layout>

<style>
  [slot="description"] > :first-child {
    margin-top: -1em;
    font-family: var(--heading-font-family);
  }
</style>
