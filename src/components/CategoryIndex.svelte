<script lang="ts">
  import { Head } from "@erbridge/website-theme";

  export let title: string;
  export let description: string | null = null;
  export let pages: {
    title: string;
    slug: string;
    extract?: string;
    summary?: string;
  }[];
</script>

<Head {title} {description} />

<h1>{title}</h1>

{#if description}
  <p>{description}</p>
{/if}

<ul>
  {#each pages as page}
    <li>
      <a sapper:prefetch href={page.slug}>
        <h2>
          {page.title}
        </h2>

        {#if page.extract}
          <p>{page.extract}…</p>
        {:else if page.summary}
          <p>{page.summary}</p>
        {/if}
      </a>
    </li>
  {/each}
</ul>

<style>
  ul {
    padding-left: 0;
    list-style: none;
  }

  li h2 {
    font-size: 1.4em;
    margin-top: 0;
    margin-bottom: 0.2em;
  }

  li p {
    max-width: 30em;
    margin: 0;
    color: rgba(var(--text-colour), 0.8);
  }

  li a {
    display: block;
    border-left: 2px double rgba(var(--text-colour), 0.4);
    padding: 0.5em 0 0.5em 1em;
    text-decoration: none;
  }

  li a:active,
  li a:focus,
  li a:focus-within,
  li a:hover {
    border-left-color: rgb(var(--accent-colour));
  }
</style>
