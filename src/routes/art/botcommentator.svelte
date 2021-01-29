<script>
  import Layout from "../../layouts/art.svelte";
</script>

<Layout
  title="@Bot&shy;Comment&shy;ator"
  description="A commentator on Twitter bot games."
>
  <div slot="description">
    <p>A commentator on Twitter bot games.</p>

    <p>
      Twitter games run by bots exist. I made <a
        rel="external"
        href="https://twitter.com/BotCommentator">@BotCommentator</a
      >
      to commentate on those games, starting with
      <a rel="external" href="https://twitter.com/massconnect4">@massconnect4</a
      >.
    </p>

    <p>
      It’s not the most intelligent commentator, but it does understand the
      game. I found it amusing. Not amusing enough to modify it for other games
      when Mass Connect 4 shut down though, apparently.
    </p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/botcommentator">here</a
      >.
    </p>
  </div>

  <a
    class="twitter-timeline"
    data-dnt="true"
    data-theme="dark"
    rel="external"
    href="https://twitter.com/BotCommentator">Tweets by BotCommentator</a
  >
  <!-- prettier-ignore-start --><script
    async
    src="https://platform.twitter.com/widgets.js"
    charset="utf-8"></script><!-- prettier-ignore-end -->
</Layout>
