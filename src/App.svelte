<script>
  import AOS from "aos";
  import { onMount } from "svelte";
  import Nav from "./components/Nav.svelte";
  import Hero from "./components/Hero.svelte";
  import Companies from "./components/Companies.svelte";
  import Sellout from "./components/Sellout.svelte";
  import Getstarted from "./components/Getstarted.svelte";
  import Trees from "./components/Trees.svelte";

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
  <Nav />
  <Hero />
  <Companies />
  <Sellout />
  <Getstarted />
  <Trees />
</div>
