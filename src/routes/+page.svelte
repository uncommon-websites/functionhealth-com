<script lang="ts">
	import Header from "$lib/components/Header.svelte";
	import Hero from "$lib/components/Hero.svelte";
	import ProcessSection from "$lib/components/ProcessSection.svelte";
	import MonitorSection from "$lib/components/MonitorSection.svelte";
	import TestsSection from "$lib/components/TestsSection.svelte";
	import StandardSection from "$lib/components/StandardSection.svelte";
	import RealPeopleSection from "$lib/components/RealPeopleSection.svelte";
	import GoldStandardSection from "$lib/components/GoldStandardSection.svelte";
	import ComparisonSection from "$lib/components/ComparisonSection.svelte";
</script>

<Header />

<main>
	<Hero />
	<ProcessSection />
	<MonitorSection />
	<TestsSection />
	<StandardSection />
	<RealPeopleSection />
	<GoldStandardSection />
	<ComparisonSection />
</main>

