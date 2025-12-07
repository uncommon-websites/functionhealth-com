<script lang="ts">
	const conditions = [
		"Mold toxicity", "Pancreatic cancer", "Lead toxicity", "Addison's disease", "Gout", "Insulin resistance", 
		"Graves' disease", "Hemochromatosis", "Anemia", "Fatty liver disease", "PCOS", "Alzheimer's"
	];
</script>

<section class="py-24 bg-[#fdfbf7] overflow-hidden">
	<div class="max-w-[1400px] mx-auto px-6 text-center mb-16">
		<h2 class="text-4xl md:text-5xl font-display mb-6 text-[#1a1a1a]">
			Monitor early indicators of <br />
			<span class="italic text-[#ce6f46]">1000s of diseases</span>
		</h2>

		<div class="flex flex-wrap justify-center gap-6 md:gap-12 text-sm text-gray-600">
			<div class="flex items-center gap-2">
				<div class="w-5 h-5 rounded-full border border-[#ce6f46] flex items-center justify-center text-[#ce6f46]">✓</div>
				Establish your long-term baseline
			</div>
			<div class="flex items-center gap-2">
				<div class="w-5 h-5 rounded-full border border-[#ce6f46] flex items-center justify-center text-[#ce6f46]">✓</div>
				Tracked for life
			</div>
			<div class="flex items-center gap-2">
				<div class="w-5 h-5 rounded-full border border-[#ce6f46] flex items-center justify-center text-[#ce6f46]">✓</div>
				Monitor how your body changes
			</div>
		</div>
	</div>

	<!-- Scrolling content and Graph -->
	<div class="relative w-full">
		<!-- Background scrolling text (simplified visual representation) -->
		<div class="flex justify-center items-center gap-8 opacity-40 whitespace-nowrap overflow-hidden py-10 mask-image-linear-gradient">
			{#each conditions as condition}
				<span class="text-xl md:text-2xl text-gray-400 font-display">{condition}</span>
				<span class="w-1 h-1 bg-gray-300 rounded-full"></span>
			{/each}
			{#each conditions as condition}
				<span class="text-xl md:text-2xl text-gray-400 font-display">{condition}</span>
				<span class="w-1 h-1 bg-gray-300 rounded-full"></span>
			{/each}
		</div>

		<!-- Central Graph Card -->
		<div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-white rounded-xl shadow-xl p-6 w-[300px] md:w-[400px] border border-gray-100">
			<div class="flex justify-between items-center mb-8">
				<div class="text-xs font-bold text-gray-400 tracking-widest uppercase">IN RANGE</div>
				<div class="text-xs font-bold text-gray-400 tracking-widest uppercase">ABOVE RANGE</div>
			</div>
			
			<div class="relative h-32">
				<!-- Grid lines -->
				<div class="absolute inset-x-0 top-0 h-px bg-gray-100"></div>
				<div class="absolute inset-x-0 bottom-0 h-px bg-gray-100"></div>
				<div class="absolute inset-x-0 top-1/2 h-px bg-green-50"></div>
				
				<!-- Green Zone -->
				<div class="absolute inset-x-0 top-0 bottom-1/2 bg-green-50/30"></div>

				<!-- Data Line -->
				<svg class="absolute inset-0 w-full h-full overflow-visible">
					<path d="M40,80 L150,40 L260,100" fill="none" stroke="#ce6f46" stroke-width="2" />
					<circle cx="40" cy="80" r="4" fill="#ce6f46" />
					<circle cx="150" cy="40" r="4" fill="#ce6f46" />
					<circle cx="260" cy="100" r="4" fill="#ce6f46" />
				</svg>

				<!-- Labels -->
				<div class="absolute bottom-0 left-[10%] transform translate-y-6 text-[10px] text-gray-400">May 25</div>
				<div class="absolute bottom-0 left-[45%] transform translate-y-6 text-[10px] text-gray-400">Oct 25</div>
				<div class="absolute bottom-0 left-[80%] transform translate-y-6 text-[10px] text-gray-400">May 26</div>
			</div>
			
			<div class="mt-8 text-xs font-bold text-red-400 tracking-widest uppercase">BELOW RANGE</div>
		</div>
	</div>
	
	<div class="max-w-[1400px] mx-auto px-6 mt-32">
		<button class="text-[10px] font-mono uppercase tracking-widest text-gray-400 hover:text-gray-600 flex items-center gap-2">
			<div class="w-2 h-2 bg-gray-400 rounded-full animate-pulse"></div>
			PAUSE MOTION
		</button>
	</div>
</section>

<style>
	.mask-image-linear-gradient {
		mask-image: linear-gradient(to right, transparent, black 20%, black 80%, transparent);
	}
</style>
