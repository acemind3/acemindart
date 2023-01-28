<script lang="ts">
    const imageLocations: string[] = ["http://placekitten.com/400/600", "http://placekitten.com/400/300", "http://placekitten.com/400/400"];
</script>

<style lang="scss">
  .gallery {
    padding: 80px 60px;
    display: flex;
    flex-wrap: wrap;
    gap: 16px;

    &__img {
      max-height: 500px;
      max-width: 400px;
    }

  }
</style>

<div id="gallery" class="gallery">
    {#each imageLocations as image}
        <img class="gallery__img" src={image} placeholder="image"/>
    {/each}
</div>