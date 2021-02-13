<script>
  import blindfield from "images/play/blindfield.jpg";
  import PageBackgroundImage from "../../../components/PageBackgroundImage.svelte";
  import Layout from "../../../layouts/play.svelte";
</script>

<Layout
  title="Blindfield"
  description="Search for treasure together in a minefield you can’t see."
>
  <div slot="description">
    <div>prototype</div>

    <p>
      A game prototype made while seasick for <a
        rel="external"
        href="https://blog.erbridge.co.uk/archive/splash-jam-2016"
        >Splash Jam 2016</a
      >.
    </p>

    <p>Made by:</p>
    <ul>
      <li>
        <a rel="external" href="https://twitter.com/aaronvark">Aaron Oostdijk</a
        >
      </li>
      <li>
        <a rel="external" href="https://twitter.com/WillR1ker">Will McMain</a>
      </li>
      <li>
        <a rel="external" href="https://twitter.com/fauxvaldemar"
          >Valdemar Andreasen</a
        >
      </li>
      <li>
        <a rel="external" href="https://twitter.com/dasmalle">Malena Klaus</a>
      </li>
      <li>me</li>
    </ul>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/SilentPanda/blindfield">here</a
      >.
    </p>
  </div>

  <p>
    This game requires an audience. Two players share an Xbox controller,
    holding one side each behind their backs. They should stand so they are
    unable to see the screen.
  </p>

  <p>
    The audience should be able to see the screen and be heard by the players
    (but turn the volume up loud).
  </p>

  <p>
    Each player controls one of the coloured circles on the screen. They both
    have metal detectors that work in different ways. One of them has a long
    range detector that vibrates when they are moving in the direction of the
    treasure, but gets weaker as it gets closer. The other has a short range
    detector that gets stronger, the closer it gets to the treasure. When both
    players are standing on the treasure, they win.
  </p>

  <p>
    The audience's job is to guide the two players, to help them find the
    treasure and each other without stepping on any mines.
  </p>

  <p>Good luck!</p>

  <p>
    Play it <a rel="external" href="https://erbridge.itch.io/memory-leak"
      >here</a
    >.
  </p>

  <PageBackgroundImage src={blindfield} />
</Layout>

<style>
  [slot="description"] > :first-child {
    margin-top: -1em;
    font-family: var(--heading-font-family);
  }

  ul {
    list-style: none;
    padding-left: 0;
    color: rgba(var(--text-colour), 0.8);
  }
</style>
