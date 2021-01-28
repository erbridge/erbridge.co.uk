<script lang="ts">
  import BaseLayout from "./base.svelte";

  export let title: string;
  export let subtitle: string | null = null;
  export let description: string | null = null;
  export let opaqueHeader = false;
</script>

<BaseLayout {title} {subtitle} {description} {opaqueHeader}>
  <meta slot="head" property="og:article:author" content="F" />
  <slot slot="description" name="description" />
  <slot />
</BaseLayout>
