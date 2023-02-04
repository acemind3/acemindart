<script lang="ts">
  import { Link } from "svelte-routing";
</script>

<div class="header">
  <Link to="/">
    <img alt="logo" />
  </Link>
</div>

<style lang="scss">
  .header {
    margin-top: 32px;
    margin-bottom: 64px;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;

    img {
      width: 64px;
      height: 64px;
    }
  }
</style>
