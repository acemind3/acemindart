<script lang="ts">
  import { Link } from "svelte-routing";
  import Footer from "../home/Footer.svelte";
  import ImagePageHeader from "../../lib/DetailPageHeader.svelte";
  import DetailPageButtons from "../../lib/DetailPageButtons.svelte";
  import ImageContainerSingle from "../../lib/DetailPageImageContainerSingle.svelte";
  import ImageContainerDouble from "../../lib/DetailPageImageContainerDouble.svelte";
</script>

<div class="adora-page">
  <ImagePageHeader />
  <ImageContainerDouble srcLeft="/Adora.png" srcRight="/Catra.png" />
  <div class="description">INSERT COOL AND AWESOME DESCRIPTION HERE</div>
  <DetailPageButtons downloadUrl="/Adora.png" />
  <Footer />
</div>

<style lang="scss">
  .description {
    width: 100%;
    text-align: center;
    margin-top: 32px;
    margin-bottom: 64px;
  }
</style>
