<script>
  import whenInRome from "images/games/when-in-rome.jpg";
  import PageBackgroundImage from "../../../components/PageBackgroundImage.svelte";
  import Layout from "../../../layouts/games.svelte";
</script>

<Layout
  title="When in Rome"
  description="The Amazon Alexa-enabled travel trivia social board game."
>
  <div slot="description">
    <div>discontinued</div>

    <p>
      A digital-physical game made at <a
        rel="external"
        href="https://nianticlabs.com/blog/sensibleobject">Sensible Object</a
      >.
    </p>
  </div>

  <p>
    When in Rome is a travel trivia social board game where Amazon Alexa asks
    the questions. Players split into two teams and race to score the most
    points and collect souvenirs from around the world.
  </p>

  <p>
    On each turn, a team chooses a connected location to fly to and answers a
    question posed by a real local about their location. Get it right, and they
    make a friend, allowing them to travel further on future turns. Get it wrong
    and they can try again on their next turn.
  </p>

  <p>
    During the game, you'll hear rumours of souvenirs somewhere in the world.
    Race to get there first and score big.
  </p>

  <p>No longer available.</p>

  <PageBackgroundImage src={whenInRome} />
</Layout>

<style>
  [slot="description"] > :first-child {
    margin-top: -1em;
    font-family: var(--heading-font-family);
  }
</style>
