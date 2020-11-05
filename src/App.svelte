<script>
  import AOS from "aos";
  import { onMount } from "svelte";
  import Nav from "./components/Nav.svelte";
  import Hero from "./components/Hero.svelte";
  import Companies from "./components/Companies.svelte";
  import Sellout from "./components/Sellout.svelte";
  import Getstarted from "./components/Getstarted.svelte";
  import Trees from "./components/Trees.svelte";
  import Pricing from "./components/Pricing.svelte";
  import Faq from "./components/Faq.svelte";
  import Honorable from "./components/Honorable.svelte";
  import Contact from "./components/Contact.svelte";
  import Footer from "./components/Footer.svelte";

  onMount(() => {
    AOS.init({
      duration: 1000,
    });
  });
</script>

<style>
</style>

<svelte:head>
  <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
</svelte:head>

<div class="wrapper">
  <div id="home">
    <Nav />
  </div>
  <Hero />
  <Companies />
  <div id="why">
    <Sellout />
  </div>
  <Getstarted />
  <div id="overview">
    <Trees />
  </div>
  <div id="pricing">
    <Pricing />
  </div>
  <div id="faq">
    <Faq />
  </div>
  <Honorable />
  <div id="contact">
    <Contact />
  </div>
  <Footer />
</div>
