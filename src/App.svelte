<script lang="ts">
    import Hero from "./lib/Hero.svelte";
    import Gallery from "./lib/Gallery.svelte";
    import TipJar from "./lib/TipJar.svelte";
    import Disclaimer from "./lib/Disclaimer.svelte";
    import Footer from "./lib/Footer.svelte";
    import BuyMeACoffee from "./lib/BuyMeACoffee.svelte";

    const imageLocations: string[] = ["http://placekitten.com/400/600", "http://placekitten.com/400/300", "http://placekitten.com/400/400"];

    const buyMeACoffeeLink = "https://www.buymeacoffee.com/ace3mind";
    const thisYear = new Date().getFullYear();
</script>

<div id="app" class="app">
    <Hero/>
    <Gallery/>
    <TipJar/>
    <Disclaimer/>
    <Footer/>
    <BuyMeACoffee/>
</div>