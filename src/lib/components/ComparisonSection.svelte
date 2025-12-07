<script lang="ts">
	const features = [
		"Lab tests annually",
		"Personalized Protocol",
		"Upload past results",
		"No insurance needed",
		"Hormones & fertility testing",
		"Heavy metal & toxin testing",
		"Metabolic & pancreatic testing",
		"Heart testing beyond cholesterol",
		"Nutrient/electrolyte testing",
		"Autoimmunity testing",
		"Thyroid testing",
		"Access to advanced MRI & CT",
		"Access to GRAIL cancer test",
		"Access to Alzheimers & brain testing",
		"Access to mold reactivity testing"
	];
</script>

<section class="py-24 bg-[#fdfbf7]">
	<div class="max-w-[1000px] mx-auto px-6">
		<h2 class="text-4xl md:text-5xl font-display text-center mb-16 text-[#1a1a1a]">
			Not your average <span class="italic text-[#ce6f46]">checkup</span>
		</h2>

		<div class="rounded-2xl overflow-hidden border border-gray-200 bg-[#f5f2eb]">
			<!-- Header -->
			<div class="grid grid-cols-12 border-b border-gray-200">
				<div class="col-span-6 p-6"></div>
				<div class="col-span-3 bg-[#ce6f46] text-white p-6 text-center">
					<div class="flex items-center justify-center gap-2 font-display text-xl">
						<div class="w-6 h-6 rounded-full border border-white flex items-center justify-center">
							<div class="w-4 h-4 bg-white opacity-20 rotate-45"></div>
						</div>
						Function
					</div>
				</div>
				<div class="col-span-3 p-6 text-center text-xs font-bold uppercase tracking-wider text-gray-500 flex items-center justify-center">
					Standard checkup
				</div>
			</div>

			<!-- First Row (Special) -->
			<div class="grid grid-cols-12 border-b border-gray-200 bg-[#f5f2eb]">
				<div class="col-span-6 p-6 text-sm font-medium text-gray-700 flex items-center">
					Lab tests annually
				</div>
				<div class="col-span-3 bg-[#b85e38] text-white p-6 flex items-center justify-center font-bold">
					160+
				</div>
				<div class="col-span-3 p-6 flex items-center justify-center font-bold text-gray-500">
					~26
				</div>
			</div>

			<!-- Other Rows -->
			{#each features.slice(1) as feature, i}
				<div class="grid grid-cols-12 border-b border-gray-200 last:border-0 hover:bg-black/5 transition-colors">
					<div class="col-span-6 p-5 md:p-6 text-sm text-gray-600 flex items-center">
						{feature}
					</div>
					<div class="col-span-3 bg-[#ce6f46]/10 p-5 md:p-6 flex items-center justify-center border-l border-r border-[#ce6f46]/20">
						<div class="w-6 h-6 rounded-full bg-[#ce6f46] text-white flex items-center justify-center text-xs">
							<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-4 h-4">
								<path fill-rule="evenodd" d="M19.916 4.626a.75.75 0 0 1 .208 1.04l-9 13.5a.75.75 0 0 1-1.154.114l-6-6a.75.75 0 0 1 1.06-1.06l5.353 5.353 8.493-12.74a.75.75 0 0 1 1.04-.207Z" clip-rule="evenodd" />
							</svg>
						</div>
					</div>
					<div class="col-span-3 p-5 md:p-6 flex items-center justify-center">
						<div class="w-6 h-6 rounded-full border border-gray-400 text-gray-400 flex items-center justify-center text-xs">
							<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="w-4 h-4">
								<path fill-rule="evenodd" d="M5.47 5.47a.75.75 0 0 1 1.06 0L12 10.94l5.47-5.47a.75.75 0 1 1 1.06 1.06L13.06 12l5.47 5.47a.75.75 0 1 1-1.06 1.06L12 13.06l-5.47 5.47a.75.75 0 0 1-1.06-1.06L10.94 12 5.47 6.53a.75.75 0 0 1 0-1.06Z" clip-rule="evenodd" />
							</svg>
						</div>
					</div>
				</div>
			{/each}
		</div>
	</div>
</section>
