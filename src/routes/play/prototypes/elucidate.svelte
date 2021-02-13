<script>
  import elucidate from "images/play/elucidate.jpg";
  import PageBackgroundImage from "../../../components/PageBackgroundImage.svelte";
  import Layout from "../../../layouts/play.svelte";
</script>

<Layout
  title="elucidate"
  description="Learn to communicate with a dream entity."
>
  <div slot="description">
    <div>prototype</div>

    <p>
      Made for <a
        rel="external"
        href="https://globalgamejam.org/2018/games/elucidate"
        >Global Game Jam 2018</a
      >
      with the talented
      <a rel="external" href="https://twitter.com/R_Michalak">Beck Michalak</a>,
      <a rel="external" href="https://twitter.com/_JakeTucker">Jake Tucker</a>,
      and
      <a rel="external" href="https://dave-allen-music.com/">Dave Allen</a>.
    </p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/elucidate">here</a
      >.
    </p>
  </div>

  <p>
    A being only reached in dreams cannot converse in human tongue. A entity
    existing in such a different plane cannot understand the whims of your kind.
    You must try to find a way to communicate with this entity while being
    restrained by it's own alien language. Arcana and pictographs reveal an
    insight into it's attitude towards you, something that you can and will
    influence over the course of the game. The goal is to bridge the gap between
    you. To change the power dynamic from ruler and subject into something else.
    How this changes is up to you.
  </p>

  <p>
    elucidate is a code-breaking game, letters correspond to glyphs generated
    anew each game and images give clues as to the words being said to you and
    their meaning. Reply how you will. Certain answers will make this being feel
    differently about you and encourage it to explore different tactics in order
    to keep the status quo. There are many different outcomes, and few end well
    for you.
  </p>

  <p>
    Play it <a rel="external" href="https://elucidate.erbridge.co.uk/">here</a>.
  </p>

  <PageBackgroundImage src={elucidate} />
</Layout>

<style>
  [slot="description"] > :first-child {
    margin-top: -1em;
    font-family: var(--heading-font-family);
  }
</style>
