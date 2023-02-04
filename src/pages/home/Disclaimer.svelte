<style lang="scss">
  $white-text: #fff;
  $disclaimer-background: #060735;
  $disclaimer-link: rgb(226, 38, 88);


  .disclaimer {
    height: 500px;
    background: $disclaimer-background;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 0 15%;
    color: $white-text;
    gap: 24px;

    &__paragraph {
      font-size: 22px;
    }

    &__link {
      color: $disclaimer-link;
    }
  }
</style>

<div class="disclaimer">
    <p class="disclaimer__paragraph">
        Since my designs are works of fanart, I cannot legally sell them. However, I’ve decided to release my hi res
        print and digital files for free! Feel free to download them, print them, or you use on your digital
        devices.

    </p>
    <p class="disclaimer__paragraph">
        Online print options include <a class="disclaimer__link" href="https://www.shutterfly.com">shutterfly</a> ,
        <a href="https://www.artifactuprising.com" class="disclaimer__link">
            artifact uprising
        </a> , <a href="https://www.fedex.com/en-us/printing/online-printing.html"
                  class="disclaimer__link">fedex</a> and many more I haven’t listed. Better
        yet, find somewhere local and support their business!
    </p>
</div>