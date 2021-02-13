<script lang="ts">
  import { Head } from "@erbridge/website-theme";
  import { quadIn } from "svelte/easing";

  export let title: string;
  export let subtitle: string | null = null;
  export let description: string | null = null;
  export let opaqueHeader = true;

  let innerWidth: number;
  let innerHeight: number;
  let scrollY: number;

  let section: HTMLElement;

  let headerOpacity = 1;

  $: if (!opaqueHeader && innerWidth && innerHeight && section) {
    const sectionTop = section.offsetTop;

    headerOpacity = quadIn(
      Math.max(
        Math.min(1 - (scrollY - sectionTop) / (innerHeight - sectionTop), 1),
        0
      )
    );
  }
</script>

<svelte:window bind:innerWidth bind:innerHeight bind:scrollY />

<Head
  title={(subtitle ? `${title}: ${subtitle}` : title).toLowerCase()}
  type="article"
  {description}
>
  <slot name="head" />
</Head>

<article>
  <header style="opacity: {headerOpacity};">
    <div>
      <h1>{title}</h1>

      {#if subtitle}
        <h2>{subtitle}</h2>
      {/if}

      <slot name="description" />
    </div>
  </header>

  <section bind:this={section}>
    <slot />
  </section>
</article>

<style>
  article {
    position: relative;
  }

  header {
    max-width: 30rem;
    margin-left: auto;
    text-align: right;
    will-change: opacity;
  }

  header :global(p) {
    max-width: 60%;
    margin-left: auto;
    color: rgba(var(--text-colour), 0.8);
  }

  section {
    overflow-x: auto;
    overflow-y: hidden;
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

    header h1 {
      hyphens: manual;
    }

    header :global(p) {
      max-width: 80%;
    }

    section {
      flex: 1;
    }
  }
</style>
