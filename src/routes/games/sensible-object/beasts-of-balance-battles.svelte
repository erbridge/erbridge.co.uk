<script>
  import beastsOfBalance from "images/games/beasts-of-balance.jpg";
  import PageBackgroundImage from "../../../components/PageBackgroundImage.svelte";
  import Layout from "../../../layouts/games.svelte";
</script>

<Layout
  title="Beasts of Balance Battles"
  description="A competitive expansion to the digital-tabletop-stacking-meets-strategy game."
>
  <div slot="description">
    <div>release</div>

    <p>
      A digital-physical game expansion made at <a
        rel="external"
        href="https://nianticlabs.com/blog/sensibleobject">Sensible Object</a
      >.
    </p>
  </div>

  <p>
    Beasts of Balance is a digital-physical game of stacking oddly shaped
    objects in the real world to evolve a digital one and score points. The base
    game is a cooperative game, where you work together to get the highest score
    (or for some players, the tallest tower). The game ends when the tower
    collapses, ending the virtual world.
  </p>

  <p>
    Battles adds a competitive game mode where two or three players take control
    of a region and try to get the highest score without knocking the tower
    over. Battles introduced a card game element, where you scan your card at
    any point to interfere with the other players or boost your own turn.
  </p>

  <p>
    Buy the game <a rel="external" href="https://shop-uk.beastsofbalance.com/"
      >here</a
    >.
  </p>

  <PageBackgroundImage src={beastsOfBalance} />
</Layout>

<style>
  [slot="description"] > :first-child {
    margin-top: -1em;
    font-family: var(--heading-font-family);
  }
</style>
