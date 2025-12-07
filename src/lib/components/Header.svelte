<script lang="ts">
	import { onMount } from 'svelte';

	let isScrolled = false;

	onMount(() => {
		const handleScroll = () => {
			isScrolled = window.scrollY > 50;
		};
		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<div class="fixed top-0 left-0 w-full z-50 transition-all duration-300 {isScrolled ? 'bg-white/90 backdrop-blur-md shadow-sm text-brand-dark' : 'bg-transparent text-white'}">
	<!-- Top Banner -->
	<div class="bg-[#c26d48] text-white text-xs font-medium py-2 text-center">
		$499 &rarr; $365. <span class="underline cursor-pointer">Gift for $1/day.</span>
	</div>

	<!-- Main Nav -->
	<div class="max-w-[1400px] mx-auto px-6 h-20 flex items-center justify-between">
		<!-- Logo -->
		<a href="/" class="flex items-center gap-2">
			<div class="w-8 h-8 rounded-full border-2 border-current flex items-center justify-center relative overflow-hidden">
				<div class="w-[120%] h-[120%] bg-current opacity-20 rotate-45 transform translate-y-1"></div>
			</div>
			<span class="text-2xl font-display font-medium tracking-tight">Function</span>
		</a>

		<!-- Links -->
		<nav class="hidden lg:flex items-center gap-8 text-sm font-medium">
			<a href="#" class="hover:opacity-80">How it works</a>
			<a href="#" class="hover:opacity-80">What we test</a>
			<a href="#" class="hover:opacity-80">Scans</a>
			<a href="#" class="hover:opacity-80">FAQ</a>
			<a href="#" class="hover:opacity-80">About</a>
		</nav>

		<!-- Right Actions -->
		<div class="flex items-center gap-6">
			<a href="#" class="text-sm font-medium hover:opacity-80 hidden sm:block">Login</a>
			<button class="bg-[#ce6f46] hover:bg-[#b85e38] text-white px-6 py-2.5 rounded-full text-sm font-medium transition-colors">
				Start testing
			</button>
			<button class="hover:opacity-80">
				<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-5 h-5">
					<path stroke-linecap="round" stroke-linejoin="round" d="m21 21-5.197-5.197m0 0A7.5 7.5 0 1 0 5.196 5.196a7.5 7.5 0 0 0 10.607 10.607Z" />
				</svg>
			</button>
			<button class="hover:opacity-80 lg:hidden">
				<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" class="w-6 h-6">
					<path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
				</svg>
			</button>
		</div>
	</div>
</div>
