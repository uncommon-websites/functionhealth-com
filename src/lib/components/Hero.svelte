<script lang="ts">
</script>

<section class="relative h-screen min-h-[700px] w-full overflow-hidden">
	<!-- Background Image -->
	<div class="absolute inset-0">
		<img 
			src="https://images.unsplash.com/photo-1476480862126-209bfaa8edc8?q=80&w=2670&auto=format&fit=crop" 
			alt="Runner in fog" 
			class="w-full h-full object-cover object-center"
		/>
		<!-- Overlay to darken and match tone -->
		<div class="absolute inset-0 bg-black/30 bg-gradient-to-b from-black/20 via-transparent to-black/60"></div>
	</div>

	<!-- Content -->
	<div class="relative z-10 h-full max-w-[1400px] mx-auto px-6 flex flex-col justify-center text-white pb-20">
		<div class="inline-block bg-white/20 backdrop-blur-sm px-3 py-1 rounded-full text-[10px] font-bold tracking-wider uppercase mb-6 w-fit">
			HSA/FSA Eligible
		</div>
		
		<h1 class="font-display text-5xl md:text-7xl lg:text-8xl italic leading-[1.1] mb-6 max-w-4xl">
			Your advanced <br />
			<span class="not-italic">health check</span>
		</h1>
		
		<p class="text-lg md:text-xl text-white/90 max-w-xl mb-10 font-light leading-relaxed">
			Every year. Starting with 160+ lab tests detecting 1000+ conditions. Just <span class="line-through opacity-70">$499</span> &rarr; $365 per year—$1 per day.
		</p>
		
		<button class="bg-white text-black px-8 py-3.5 rounded-full font-medium hover:bg-gray-100 transition-colors w-fit text-sm md:text-base">
			Start testing
		</button>
	</div>

	<!-- Bottom Stats -->
	<div class="absolute bottom-0 left-0 w-full border-t border-white/20 bg-black/20 backdrop-blur-sm">
		<div class="max-w-[1400px] mx-auto px-6 py-6 grid grid-cols-2 md:grid-cols-4 gap-8 text-white">
			<div>
				<div class="font-bold text-lg">160+ lab tests</div>
				<div class="text-sm text-white/70">Detect 1k+ diseases</div>
			</div>
			<div>
				<div class="font-bold text-lg">2x per year</div>
				<div class="text-sm text-white/70">Track for life</div>
			</div>
			<div>
				<div class="font-bold text-lg">No insurance</div>
				<div class="text-sm text-white/70">Transparent cost</div>
			</div>
			<div class="flex justify-end items-center">
				<button class="w-10 h-10 rounded-full border border-white/30 flex items-center justify-center hover:bg-white/10 transition-colors">
					<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-4 h-4">
						<path fill-rule="evenodd" d="M4.5 5.653c0-1.426 1.529-2.33 2.779-1.643l11.54 6.348c1.295.712 1.295 2.573 0 3.285L7.28 19.991c-1.25.687-2.779-.217-2.779-1.643V5.653Z" clip-rule="evenodd" />
					</svg>
				</button>
			</div>
		</div>
	</div>
</section>
