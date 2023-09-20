<script lang="ts">
	import { page } from "$app/stores";
	import { ErrorPage } from "@erbridge/website-theme";
</script>

<ErrorPage status={$page.status} error={$page.error} />
