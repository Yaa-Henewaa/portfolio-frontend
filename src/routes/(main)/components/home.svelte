<script>
	import About3 from '$lib/images/doodle items (1).png';
	import About4 from '$lib/images/Group 62.png';
	import Csharp from '$lib/images/devicon_csharp.png';
	import svelte from '$lib/images/devicon_svelte.png';
	import tailwind from '$lib/images/devicon_tailwindcss.png';
	import html from '$lib/images/logos_html-5.png';
	import node from '$lib/images/logos_nodejs.png';

</script>

<div class="h-full w-full ">
	<div class="flex  p-5 ">
		<div class="m-12 flex w-full items-center justify-evenly gap-8 border-t border-gray-300">

			<div class="w-full ml-10 relative lg:w-2/5">
				<img class=" h-auto w-full object-contain" src={About3} alt="about " />
				<img src={About4} alt="Overlay" class="absolute top-7 left-7 w-full h-auto">
			</div>

            <div class="w-full space-y-5 py-8 lg:w-3/5 m-[10rem]">

                <div class="flex">
                    <p class=" text-5xl font-semibold">About <span class="text-[#FF64B4]">me.</span> </p> 
 
                </div>
				<p class=" w-full text-lg">
					I'm passionate about building scalable, efficient, and user-friendly
					software solutions. With expertise in backend systems, web development, and machine
					learning, I thrive on solving problems and delivering impactful results.
				</p>
			</div>
		</div>

	</div>
	<div class="flex h-20">
		<div class=" mx-[8rem] flex h-full w-full items-center justify-evenly space-x-12 border-y border-gray-300">
			<img class=" h-auto w-10 max-w-full object-contain" src={Csharp} alt="behance" />
			<img class=" h-auto w-10 max-w-full object-contain" src={svelte} alt="Google" />
			<img class=" h-auto w-[3rem] max-w-full object-contain" src={tailwind} alt="apple" />
			<img class=" h-auto w-[4rem] max-w-full object-contain" src={node} alt="Dribble" />
			<img class=" h-auto w-[2rem] object-contain" src={html} alt="awwwarrds" />
		</div>
	</div>

</div>
