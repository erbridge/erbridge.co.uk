<script lang="ts">
  export let src: string;
</script>

<div class="container">
  <img role="presentation" {src} alt="" />
  <div />
</div>

<style>
  .container {
    width: 100vw;
    max-height: 100vh;
    position: fixed;
    left: 0;
    bottom: 0;
    z-index: -1;
    opacity: 0.2;
    overflow: hidden;
  }

  .container img {
    width: 100%;
    display: block;
  }

  .container div {
    width: 100%;
    position: absolute;
    bottom: 0;
    top: 0;
    background: linear-gradient(
      to bottom,
      rgb(var(--background-colour)) 0%,
      transparent 100%
    );
  }
</style>
