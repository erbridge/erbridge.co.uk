<script lang="ts">
  import { Head } from "@erbridge/website-theme";
  import PageLinkList from "./PageLinkList.svelte";

  export let title: string;
  export let description: string | null = null;
  export let pages: {
    title: string;
    slug: string;
    extract?: string;
    summary?: string;
    background?: string;
  }[];
</script>

<Head {title} {description} />

<h1>{title}</h1>

{#if description}
  <p>{description}</p>
{/if}

<PageLinkList {pages} />
