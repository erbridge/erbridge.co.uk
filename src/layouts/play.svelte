<script lang="ts">
  import BaseLayout from "./base.svelte";

  export let title: string;
  export let subtitle: string | null = null;
  export let description: string | null = null;
  export let opaqueHeader = true;
</script>

<BaseLayout {title} {subtitle} {description} {opaqueHeader}>
  <slot slot="head" name="head" />
  <slot slot="description" name="description" />
  <slot />
</BaseLayout>
