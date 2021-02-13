<script lang="ts">
  export let src: string;
  export let type: "main" | "description" = "main";
</script>

<div class="container {type}">
  <img role="presentation" {src} alt="" />
  <div />
</div>

<style>
  .description {
    margin-top: -4em;
  }

  .main {
    display: none;
  }

  .container {
    width: 100%;
    max-height: 80vh;
    position: absolute;
    left: 0;
    z-index: -1;
    opacity: 0.1;
    overflow: hidden;
  }

  .container img {
    width: 100%;
  }

  .container div {
    width: 100%;
    position: absolute;
    bottom: 0;
    top: 0;
    box-shadow: 0 0 15vw 15vw rgb(var(--background-colour)) inset;
  }

  @media (min-width: 700px) {
    .description {
      display: none;
    }

    .main {
      display: block;
    }
  }
</style>
