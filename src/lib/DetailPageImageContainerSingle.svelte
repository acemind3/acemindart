<script lang="ts">
  export let src: string = "";
</script>

<div class="image-container-single-variant">
  <img alt="adora" {src} />
</div>

<style lang="scss">
  .image-container-single-variant {
    width: 100%;
    display: flex;
    justify-content: center;

    img {
      width: 50%;
    }
  }
</style>
