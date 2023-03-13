<div class="under-construction">
  <div class="under-construction__overlay" />
  <a class="under-construction__logo">
    <img src="./Logo-white.png" placeholder="logo" />
  </a>
  <h1 class="under-construction__header">Site Under Construction</h1>
</div>

<style lang="scss">
  @import "../../global.scss";

  $white-text: #fff;
  $overlay: #430b9e;
  $hero-img: url("/jinx-website-wallpaper.png");

  .under-construction {
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #323232;
    min-height: 100vh;
    background: $hero-img;
    background-size: cover;

    &__overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: $overlay;
      opacity: 0.65;
      z-index: 0;
    }

    &__logo {
      z-index: 1;
      margin-bottom: 150px;
      margin-top: 40px;

      &:hover {
        opacity: 0.5;
      }
    }

    &__header {
      font-size: 6rem;
      text-align: center;
      color: #fafafa;
      z-index: 1;
      font-weight: 600;

      @include smallBreakpoint {
        font-size: 4rem;
      }
    }
  }
</style>
