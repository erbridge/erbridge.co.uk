<script>
  import Layout from "../../layouts/art.svelte";
</script>

<Layout
  title="SEED DISPERSAL"
  description="A walk through Project Gutenberg, one paragraph at a time, created for NaNoGenMo 2015."
>
  <div slot="description">
    <p>Version 0.0.2</p>

    <p>
      A walk through <a rel="external" href="https://www.gutenberg.org/"
        >Project Gutenberg</a
      >, one paragraph at a time, created for
      <a rel="external" href="https://github.com/dariusk/NaNoGenMo-2015"
        >NaNoGenMo 2015</a
      >.
    </p>

    <p>
      We start at a chosen book’s <var>ID</var>. We find the <var>ID</var>th
      paragraph from that book, and add it. We then calculate the sum of the
      unicode values of the characters in that paragraph, and use that total as
      the <var>ID</var> of the next book.
    </p>

    <p>
      You can read earlier versions and the source code that generates this
      novel, here:
    </p>

    <ul>
      <li>
        <a
          rel="external"
          href="https://cdn.rawgit.com/erbridge/seed-dispersal/master/dist/seed-dispersal-0.0.1.pdf"
          >Version 0.0.1</a
        >
      </li>
      <li>
        <a rel="external" href="https://github.com/erbridge/seed-dispersal"
          >Source</a
        >
      </li>
    </ul>
  </div>

  <div class="pdf">
    <object
      aria-label="SEED DISPERSAL"
      role="document"
      data="https://cdn.rawgit.com/erbridge/seed-dispersal/master/dist/seed-dispersal-0.0.2.pdf"
      type="application/pdf"
    />

    <p>
      <a
        role="button"
        href="https://cdn.rawgit.com/erbridge/seed-dispersal/master/dist/seed-dispersal-0.0.2.pdf"
        >Download the PDF</a
      >
    </p>
  </div>
</Layout>

<style>
  var {
    font-family: var(--monospace-font-family);
    font-style: unset;
  }

  ul {
    margin-top: 0;
    margin-left: 0;
    padding-left: 0;
    list-style: none;
    color: rgba(var(--text-colour), 0.8);
  }

  .pdf {
    height: 100%;
    display: flex;
    flex-direction: column;
  }

  object {
    width: 100%;
    min-height: 400px;
    max-height: 90vh;
    flex-grow: 1;
  }
</style>
