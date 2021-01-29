<script>
  import Layout from "../../layouts/art.svelte";
</script>

<Layout title="@elbow&shy;noises" description="A noisy Twitter bot.">
  <div slot="description">
    <p>A noisy Twitter bot.</p>

    <p>
      Ever since I broke my arm, it sometimes makes some crunching, clicking
      noises. While it ran, this bot mimicked those noises.
    </p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/elbownoises">here</a
      >.
    </p>
  </div>

  <a
    class="twitter-timeline"
    data-dnt="true"
    data-theme="dark"
    rel="external"
    href="https://twitter.com/elbownoises">Tweets by Elbow Noises</a
  >
  <!-- prettier-ignore-start --><script
    async
    src="https://platform.twitter.com/widgets.js"
    charset="utf-8"></script><!-- prettier-ignore-end -->
</Layout>
