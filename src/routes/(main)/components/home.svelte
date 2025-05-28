<script>
	import About3 from '$lib/images/doodle items (1).png';
	import About4 from '$lib/images/Group 62.png';
	import Csharp from '$lib/images/devicon_csharp.png';
	import svelte from '$lib/images/devicon_svelte.png';
	import tailwind from '$lib/images/devicon_tailwindcss.png';
	import html from '$lib/images/logos_html-5.png';
	import node from '$lib/images/logos_nodejs.png';
</script>

<div class="h-full w-full">
	<!-- Main About Section -->
	<div class="flex flex-col lg:flex-row p-4 sm:p-6 lg:p-8 mb-12 sm:mb-16 lg:mb-20">
		<div class="flex flex-col lg:flex-row w-full items-center justify-center lg:justify-evenly gap-6 lg:gap-8 border-t border-gray-300 pt-8 lg:pt-12 px-4 sm:px-6 lg:px-12">
			
			<!-- Image Section -->
			<div class="w-full max-w-xs sm:max-w-sm lg:max-w-none lg:w-2/5 relative order-2 lg:order-1">
				<img class="h-auto w-full object-contain" src={About3} alt="about" />
				<img src={About4} alt="Overlay" class="absolute top-3 left-3 sm:top-4 sm:left-4 lg:top-7 lg:left-7 w-full h-auto" />
			</div>

			<!-- Text Section -->
			<div class="w-full lg:w-3/5 space-y-4 sm:space-y-5 py-4 sm:py-6 lg:py-8 order-1 lg:order-2 text-center lg:text-left">
				<div class="flex justify-center lg:justify-start">
					<p class="text-3xl sm:text-4xl lg:text-5xl font-semibold">
						About <span class="text-[#FF64B4]">me.</span>
					</p>
				</div>
				<p class="w-full text-base sm:text-lg max-w-none lg:max-w-full mx-auto lg:mx-0">
					I'm passionate about building scalable, efficient, and user-friendly
					software solutions. With expertise in backend systems, web development, and machine
					learning, I thrive on solving problems and delivering impactful results.
				</p>
			</div>
		</div>
	</div>

	<!-- Technology Icons Section -->
	<div class="flex h-auto sm:h-20 py-6 sm:py-0">
		<div class="mx-4 sm:mx-[4rem] lg:mx-[8rem] flex flex-wrap sm:flex-nowrap w-full items-center justify-center sm:justify-evenly gap-6 sm:gap-8 lg:gap-12 border-y border-gray-300 py-4 sm:py-0">
			<img class=" h-8 w-10 max-w-full object-contain" src={Csharp} alt="behance" />
			<img class=" h-8 w-10 max-w-full object-contain" src={svelte} alt="Google" />
			<img class=" h-8 w-[3rem] max-w-full object-contain" src={tailwind} alt="apple" />
			<img class=" h-8 w-[4rem] max-w-full object-contain" src={node} alt="Dribble" />
			<img class=" h-8 w-[2rem] object-contain" src={html} alt="awwwarrds" />
		</div>
	</div>
</div>