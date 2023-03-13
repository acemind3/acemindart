<script lang="ts">
  interface ImageLinkPair {
    src: string;
    link: string;
  }

  import { Link } from "svelte-routing";

  const imageLocations: ImageLinkPair[] = [
    {
      src: "Adora.png",
      link: "adora",
    },
    {
      src: "Catra.png",
      link: "adora",
    },
    {
      src: "prime_web.jpg",
      link: "",
    },
    {
      src: "duel-web.png",
      link: "",
    },
    {
      src: "bmblb_glitch_16x20_small-web.jpg",
      link: "",
    },
    {
      src: "bmblb_ios-promo_website.jpg",
      link: "",
    },
    {
      src: "red-like-roses_thumbnail_rgb.jpg",
      link: "",
    },
    {
      src: "jinx_web.png",
      link: "",
    },
    {
      src: "Wednesday_web.png",
      link: "",
    },
  ];
</script>

<div id="gallery" class="gallery">
  {#each imageLocations as image}
    <Link to="/{image.link}">
      <img class="gallery__img" src={image.src} placeholder="image" />
    </Link>
  {/each}
</div>

<style lang="scss">
  .gallery {
    padding: 80px 60px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 16px;

    &__img {
      max-height: 500px;
      max-width: 400px;
      transition: all 0.2s ease-in;
      &:hover {
        box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.8);
        transform: translateX(2px) translatey(2px);
      }
    }
  }
</style>
