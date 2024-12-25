<script>
	// Import Svelte components and other necessary modules
	// import { onMount } from 'svelte';
	// import SomeComponent from './SomeComponent.svelte';
</script>

<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
	<div class="flex flex-col md:flex-row md:space-x-6 space-y-6 md:space-y-0 pb-4">
		<!-- First Card -->
		<div
			class="group w-full md:w-1/3 bg-slate-800 rounded-lg border border-gray-700 overflow-hidden border-2 border-violet-400/30 hover:border-violet-700 transition-colors duration-200"
		>
			<div class="p-4">
				<div class="aspect-w-16 aspect-h-9">
					<iframe
						class="w-full h-full rounded-md border-2 border-violet-400/30 hover:border-violet-700 transition-colors duration-200"
						src="https://www.youtube-nocookie.com/embed/IYmS16ruXp8?controls=0&modestbranding=1"
						title="YouTube video player"
						frameborder="0"
						allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
						allowfullscreen
					/>
				</div>
				<div class="mt-4 border-t border-gray-700 pt-4">
					<h3
						class="text-xl font-bold text-violet-400 group-hover:text-white mb-2 transition-colors duration-200"
					>
						Bitcoin News Spotlight: Introducing Lightning Bounties
					</h3>
					<p class="text-gray-300 text-sm">
						Watch as I present Lightning Bounties on Bitcoin News, reaching over 20k viewers
						worldwide and showcasing our revolutionary platform.
					</p>
				</div>
			</div>
		</div>

		<!-- Second Card -->
		<div
			class="group w-full md:w-1/3 bg-slate-800 rounded-lg border border-gray-700 overflow-hidden border-2 border-violet-400/30 hover:border-violet-700 transition-colors duration-200"
		>
			<div class="p-4">
				<div class="aspect-w-16 aspect-h-9">
					<iframe
						class="w-full h-full rounded-md border-2 border-violet-400/30 hover:border-violet-700 transition-colors duration-200"
						src="https://www.youtube-nocookie.com/embed/yxv3VpxuIFU?controls=0&disablekb=1&modestbranding=1"
						title="YouTube video player"
						referrerpolicy="strict-origin-when-cross-origin"
						allowfullscreen
					/>
				</div>
				<div class="mt-4 border-t border-gray-700 pt-4">
					<h3
						class="text-xl font-bold text-violet-400 group-hover:text-white mb-2 transition-colors duration-200"
					>
						Pitching Lightning Bounties at PlebLab Startup Day 2024
					</h3>
					<p class="text-gray-300 text-sm">
						See me and Enrique unveil Lightning Bounties to the Bitcoin developer community,
						demonstrating how we're reshaping open-source incentives.
					</p>
				</div>
			</div>
		</div>

		<!-- Third Card -->
		<div
			class="group w-full md:w-1/3 bg-slate-800 rounded-lg border border-gray-700 overflow-hidden border-2 border-violet-400/30 hover:border-violet-700 transition-colors duration-200"
		>
			<div class="p-4">
				<div class="aspect-w-16 aspect-h-9">
					<iframe
						class="w-full h-full rounded-md border-2 border-violet-400/30 hover:border-violet-700 transition-colors duration-200"
						src="https://www.youtube-nocookie.com/embed/qdU0iNvpdXo?controls=0&disablekb=1&modestbranding=1"
						title="YouTube video player"
						referrerpolicy="strict-origin-when-cross-origin"
						allowfullscreen
					/>
				</div>
				<div class="mt-4 border-t border-gray-700 pt-4">
					<h3
						class="text-xl font-bold text-violet-400 group-hover:text-white mb-2 transition-colors duration-200"
					>
						Winning the MIT Bitcoin Hackathon 2024
					</h3>
					<p class="text-gray-300 text-sm">
						Witness our team's triumphant moment as we clinch victory at the prestigious MIT Bitcoin
						Hackathon with Lightning Bounties.
					</p>
				</div>
			</div>
		</div>
	</div>
</div>

<style>
	.aspect-w-16 {
		position: relative;
		padding-bottom: 56.25%; /* 16:9 Aspect Ratio */
	}
	.aspect-w-16 iframe {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
	}
</style>
