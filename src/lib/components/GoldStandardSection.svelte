<section class="py-24 bg-[#fdfbf7]">
	<div class="max-w-[1400px] mx-auto px-6 grid lg:grid-cols-3 gap-12">
		<!-- Text Content -->
		<div class="lg:col-span-1">
			<h2 class="text-4xl md:text-5xl font-display text-[#1a1a1a] mb-6">
				Gold standard <br />
				<span class="italic text-[#ce6f46]">for lab testing</span>
			</h2>
			<p class="text-gray-600 mb-12 leading-relaxed">
				Labs trusted by the medical community. No startup labs. No unreliable at-home blood draws.
			</p>
			
			<div class="flex items-center gap-8 opacity-60 grayscale">
				<!-- Quest Logo Placeholder -->
				<div class="flex items-center gap-2 font-bold text-xl">
					<div class="w-8 h-8 bg-green-600 rounded-full"></div>
					Quest
				</div>
				<!-- GRAIL Logo Placeholder -->
				<div class="font-bold text-xl tracking-widest">GRAIL</div>
			</div>
		</div>

		<!-- Map Card -->
		<div class="bg-[#fdfbf7] border border-gray-200 rounded-xl p-8 flex flex-col h-[400px]">
			<div class="text-xs font-bold text-[#ce6f46] mb-4">2,000+ lab test locations <span class="text-gray-400 font-normal">across the US</span></div>
			
			<div class="flex-1 flex items-center justify-center relative">
				<!-- Simplified Dot Map of US -->
				<div class="w-full h-full relative opacity-30">
					{#each Array(100) as _, i}
						<div 
							class="absolute w-1 h-1 bg-[#ce6f46] rounded-full"
							style="top: {Math.random() * 80 + 10}%; left: {Math.random() * 90 + 5}%"
						></div>
					{/each}
				</div>
				<div class="absolute bottom-4 left-4 text-5xl md:text-6xl text-gray-400 font-light">2,000</div>
			</div>
		</div>

		<!-- Chart Card -->
		<div class="bg-[#fdfbf7] border border-gray-200 rounded-xl p-8 flex flex-col h-[400px]">
			<div class="text-xs font-bold text-[#ce6f46] mb-4">50+ million results <span class="text-gray-400 font-normal">delivered to Function members</span></div>
			
			<div class="flex-1 flex flex-col justify-end">
				<div class="text-5xl md:text-6xl text-gray-400 font-light mb-8">50M+</div>
				
				<!-- Bar Chart -->
				<div class="flex items-end gap-2 h-32">
					<div class="w-full bg-[#e8cdbf] rounded-t-sm h-[10%]"></div>
					<div class="w-full bg-[#e3c2b1] rounded-t-sm h-[20%]"></div>
					<div class="w-full bg-[#deb6a3] rounded-t-sm h-[30%]"></div>
					<div class="w-full bg-[#d9aa95] rounded-t-sm h-[40%]"></div>
					<div class="w-full bg-[#d49e87] rounded-t-sm h-[50%]"></div>
					<div class="w-full bg-[#cf9279] rounded-t-sm h-[60%]"></div>
					<div class="w-full bg-[#ca866b] rounded-t-sm h-[70%]"></div>
					<div class="w-full bg-[#c57a5d] rounded-t-sm h-[80%]"></div>
					<div class="w-full bg-[#c06e4f] rounded-t-sm h-[90%]"></div>
					<div class="w-full bg-[#ce6f46] rounded-t-sm h-[100%]"></div>
				</div>
				<div class="flex justify-between text-[10px] text-gray-400 mt-2">
					<span>50M</span>
					<span>25M</span>
				</div>
			</div>
		</div>
	</div>
</section>
