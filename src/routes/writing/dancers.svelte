<script>
  import Layout from "../../layouts/writing.svelte";
</script>

<Layout title="dancers" opaqueHeader>
  <div slot="description">
    <p>
      This poem was published in
      <cite
        ><a
          rel="external"
          href="https://www.lulu.com/en/gb/shop/zali-krishna/open-polyversity-four/paperback/product-mmj82j.html"
          >Open Polyversity 4</a
        ></cite
      >. I receive a share of any profits from sales.
    </p>

    <p>
      When reciting this poem, each line of the square should be read by a
      second reader at the same time as the line it interrupts.
    </p>
  </div>

  <!-- svelte-ignore a11y-media-has-caption -->
  <audio controls preload="metadata">
    <source src="assets/dancers.mp3" type="audio/mpeg" />
    <p>
      Your browser doesn't support HTML5 audio. You can download the recording
      from
      <a href="assets/dancers.mp3">here</a> instead.
    </p>
  </audio>

  <pre>Cold skin, warm heart.
On a pedestal, exposed. Seen.
Curves and motion examined.
Eyes and minds, dancing the lines.
Free flowing.
Flowing free.</pre>

  <div class="container">
    <pre>Merci. It starts with a kiss.
<span class="pre-square">Turns </span>taken. Rules broken.
<span class="pre-square">A line </span>from one hand to the next.
<span class="pre-square">Follow</span>ed. Inspired. Ignored.
<span class="pre-square">Libera</span>ted.
Five gestures.
One movement.</pre>

    <pre
      aria-label="the square"
      class="square">the square
divides us
reflects us
connects us</pre>
  </div>

  <pre>Cold skin, warm heart.
On a pedestal, stripped bare.
Transformed.</pre>

  <aside class="visually-hidden">
    <p>
      If you used assistive technology to read this poem, I'd love your feedback
      on whether it worked well for you. Please <a
        rel="external me"
        href="https://twitter.com/erbridge">tweet or DM me</a
      >
      or
      <a href="mailto:a11y@erbridge.co.uk">send me an email</a>.
    </p>
  </aside>
</Layout>

<style>
  audio {
    width: 100%;
    display: block;
  }

  pre {
    font-family: var(--body-font-family);
    white-space: pre-line;
  }

  .container {
    position: relative;
  }

  .square {
    width: 5.2em;
    width: calc(4em * var(--base-line-height));
    margin: 0;
    position: absolute;
    top: 1.3em;
    top: calc(1em * var(--base-line-height));
    left: 3.5em;
    text-align: justify;
    text-align-last: justify;
    text-justify: distribute;
    color: rgb(var(--accent-colour));
    font-style: italic;
  }

  .pre-square {
    width: 3em;
    margin-right: 6.2em;
    margin-right: calc(1em + 4em * var(--base-line-height));
    display: inline-block;
    text-align-last: justify;
    text-justify: distribute;
  }
</style>
