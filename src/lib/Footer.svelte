<style lang="scss">
  $white-text: #fff;
  $footer-background: rgb(42, 59, 84);


  .footer {
    background-color: $footer-background;
    color: $white-text;
    padding: 24px 12px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 16px;

    &__text {
      font-size: 14px;
    }

    &__link {
      color: $white-text;
      text-decoration: none;
      font-size: 14px;
      text-transform: uppercase;
      margin-right: 69px;
    }
  }
</style>

<script lang="ts">
    const thisYear = new Date().getFullYear();
</script>

<footer class="footer">
    <p class="footer__text">
        © {thisYear} ace3mind
    </p>
    <a href="#app" class="footer__text footer__link">
        To the top ↑
    </a>
</footer>