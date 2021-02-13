<script lang="ts">
  import { BaseLayout } from "@erbridge/website-theme";

  export let segment: string;

  const internalLinks: {
    href: string;
    segment: string | undefined;
    label?: string;
  }[] = [
    { href: ".", segment: undefined, label: "me" },
    { href: "play", segment: "play" },
    { href: "writing", segment: "writing" },
    { href: "art", segment: "art" },
  ];
  const externalLink = {
    href: "https://blog.erbridge.co.uk",
    label: "blog",
  };
</script>

<BaseLayout
  {segment}
  contactEmail="hello@erbridge.co.uk"
  {internalLinks}
  {externalLink}
>
  <slot slot="main" />
</BaseLayout>
