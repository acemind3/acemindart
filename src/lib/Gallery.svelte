<script lang="ts">
    const imageLocations: string[] = ["Adora.png", "Catra.png", "prime_web.jpg", "duel-web.png", "bmblb_glitch_16x20_small-web.jpg", "bmblb_ios-promo_website.jpg", "red-like-roses_thumbnail_rgb.jpg", "jinx_web.png", "Wednesday_web.png"];
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