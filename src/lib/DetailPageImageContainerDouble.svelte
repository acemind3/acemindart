<script lang="ts">
  export let srcLeft: string = "";
  export let srcRight: string = "";
</script>

<div class="image-container-double-variant">
  <img alt="left" src="/acemindart/{srcLeft}" />
  <img alt="right" src="/acemindart/{srcRight}" />
</div>

<style lang="scss">
  .image-container-double-variant {
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 24px;

    img {
      width: 30%;
    }
  }
</style>
