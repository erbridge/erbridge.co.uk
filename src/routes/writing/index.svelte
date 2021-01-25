<script lang="ts">
  import { Head } from "@erbridge/website-theme";

  const pages = [{ title: "USER ERROR", slug: "writing/user-error" }];
</script>

<Head title="writing" />

<ul>
  {#each pages as page}
    <li>
      <a sapper:prefetch href={page.slug}>
        <h2>
          {page.title}
        </h2>
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
