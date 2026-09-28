<script lang="ts">
	import BeforeFoundAfter from '$lib/components/BeforeFoundAfter.svelte';
	import Footer from '$lib/components/Footer.svelte';
import Header from '$lib/components/Header.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import HowItWorks from '$lib/components/HowItWorks.svelte';
	import ProofMetrics from '$lib/components/ProofMetrics.svelte';
	import Slider from '$lib/components/Slider.svelte';
	import TheActualDelivirable from '$lib/components/TheActualDelivirable.svelte';
</script>

<svelte:head>
	<title>PlanSmart — Permit Review Made Smarter</title>
	<meta
		name="description"
		content="PlanSmart helps builders, architects, and permit professionals catch potential permit issues before they become costly delays."
	/>
</svelte:head>

<Header />

<main>
	<Hero />
	<BeforeFoundAfter/>
	<Slider></Slider>
	<ProofMetrics/>
	<HowItWorks/>
	<TheActualDelivirable/>
</main>

<Footer/>
