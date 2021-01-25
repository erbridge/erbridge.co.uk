<script lang="ts">
  import { Head } from "@erbridge/website-theme";

  export let title: string;
  export let description: string;
</script>

<Head title={title.toLowerCase()} type="article" {description}>
  <meta property="og:article:author" content="F" />
</Head>

<article>
  <header>
    <div>
      <h1>{title}</h1>

      <slot name="description" />
    </div>
  </header>

  <section>
    <slot />
  </section>
</article>

<style>
  header {
    max-width: 30rem;
    margin-left: auto;
    text-align: right;
  }

  header :global(p) {
    max-width: 60%;
    margin-left: auto;
    color: rgba(var(--text-colour), 0.8);
  }

  @media (min-width: 700px) {
    article {
      display: flex;
    }

    header {
      max-width: 14rem;
      margin-right: 2rem;
      word-wrap: break-word;
    }

    header > div {
      margin-top: -0.2em;
      border-right: 2px solid rgb(var(--accent-colour));
      padding: 0.2em 1em 3em 0;
      position: sticky;
      top: 0.8em;
      will-change: transform;
    }

    header :global(p) {
      max-width: 80%;
    }

    section {
      flex: 1;
    }
  }
</style>
