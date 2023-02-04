<div class="hero">
  <div class="hero__overlay" />
  <a class="hero__logo">
    <img src="./Logo-white.png" placeholder="logo" />
  </a>
  <div class="hero__cta">
    <h1 class="hero__cta_text">Downloads</h1>
    <a href="#gallery">
      <svg
        class="hero__cta_link"
        aria-hidden="true"
        role="img"
        focusable="false"
        xmlns="http://www.w3.org/2000/svg"
        width="22"
        height="24"
        viewBox="0 0 22 24"
      >
        <polygon
          fill="%23FFF"
          points="721.105 856 721.105 874.315 728.083 867.313 730.204 869.41 719.59 880 709 869.41 711.074 867.313 718.076 874.315 718.076 856"
          transform="translate(-709 -856)"
        />
      </svg>
    </a>
  </div>
</div>

<style lang="scss">
  $white-text: #fff;
  $overlay: #430b9e;
  $hero-img: url("./jinx-website-wallpaper.png");

  .hero {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    justify-content: space-between;
    align-items: center;
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
      margin-top: 20px;

      &:hover {
        opacity: 0.5;
      }
    }

    &__cta {
      z-index: 1;
      margin-bottom: 24px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 16px;

      &_text {
        color: $white-text;
        font-size: 24px;
        font-weight: 700;
        text-align: center;
      }

      &_link {
        fill: $white-text;
        font-size: 16px;
        font-weight: 700;
        text-decoration: none;
        padding: 8px 16px;
        transition: all 0.2s ease-in-out;
        cursor: pointer;

        &:hover {
          transform: translateY(4px);
        }
      }
    }
  }
</style>
