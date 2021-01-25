<script lang="ts">
  import { ErrorPage } from "@erbridge/website-theme";

  export let status: number;
  export let error: Error;
</script>

<ErrorPage {error} {status} />
