<script lang="ts">
  import TipJar from "./TipJar.svelte";
  export let downloadUrl: string = "";
</script>

<div class="bottom-section">
  <div class="download">
    <p>Poster download here or some shit</p>
    <a href={downloadUrl} download class="download__button">Download</a>
  </div>
  <TipJar shouldBeSmall />
</div>

<style lang="scss">
  $disclaimer-background: #060735;

  .download {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 12px;
    background-color: $disclaimer-background;
    color: #ffffff;

    &__button {
      background-color: red;
      font-size: 20px;
      cursor: pointer;
      display: flex;
      align-items: center;
      padding: 8px 32px;
      border-radius: 80px;
      color: blue;
      transition: all 0.2s ease-in-out;
      text-decoration: none;
    }
  }

  .bottom-section {
    display: flex;

    > * {
      width: 50%;
    }
  }
</style>
