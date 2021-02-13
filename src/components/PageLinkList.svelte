<script lang="ts">
  export let pages: {
    title: string;
    slug: string;
    extract?: string;
    summary?: string;
    background?: string;
  }[];
  export let headingLevel: 2 | 3 = 2;
</script>

<ul>
  {#each pages as page}
    <li>
      <a sapper:prefetch href={page.slug}>
        {#if page.background}
          <div>
            <img role="presentation" src={page.background} alt="" />
          </div>
        {/if}

        {#if headingLevel === 2}
          <h2>
            {page.title}
          </h2>
        {:else if headingLevel === 3}
          <h3>
            {page.title}
          </h3>
        {/if}

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

  li {
    position: relative;
  }

  li h2,
  li h3 {
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

  li div {
    height: 100%;
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    opacity: 0.1;
    overflow: hidden;
  }

  li div img {
    width: 100%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
</style>
