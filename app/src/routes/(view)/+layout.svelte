<script lang="ts">
	import Footer from '../../components/staticDirs/Footer.svelte';
	import Header from '../../components/staticDirs/Header.svelte';
	import Hero from '../../components/staticDirs/Hero.svelte';

	let { children } = $props();
</script>

<div class="bg-gradient-to-b from-[#EDF6FF] via-[#C3B7FF] to-[#8979FF]">
	<Header />
	<Hero />
</div>
{@render children()}
<Footer />

