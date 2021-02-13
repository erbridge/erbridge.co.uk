<script lang="ts">
  export let src: string;
</script>

<div class="container">
  <img role="presentation" {src} alt="" />
  <div />
</div>

<style>
  .container {
    width: 100%;
    max-height: 80vh;
    position: absolute;
    left: 0;
    top: 0;
    z-index: -1;
    opacity: 0.1;
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
    box-shadow: 0 0 15vw 15vw rgb(var(--background-colour)) inset;
  }
</style>
