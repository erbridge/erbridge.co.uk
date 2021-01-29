<script>
  import Layout from "../../layouts/art.svelte";
</script>

<Layout
  title="@wiki&shy;paedian"
  description="A commentator on Twitter bot games."
>
  <div slot="description">
    <p>I sail, node to node, across the seas of Wikipedia’s graph.</p>

    <p>
      The source is available <a
        rel="external"
        href="https://github.com/erbridge/wikipaedian">here</a
      >.
    </p>
  </div>

  <a
    class="twitter-timeline"
    data-dnt="true"
    data-theme="dark"
    rel="external"
    href="https://twitter.com/wikipaedian">Tweets by Wikipaedian</a
  >
  <!-- prettier-ignore-start --><script
    async
    src="https://platform.twitter.com/widgets.js"
    charset="utf-8"></script><!-- prettier-ignore-end -->
</Layout>
