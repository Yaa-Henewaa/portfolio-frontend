<script lang='ts'>
	import Card from '$lib/components/shared/card.svelte';
	import ImagePlaceholder from '$lib/images/macbook.png';
	import dotnet from '$lib/images/devicon_dotnetcore.png';
	import jupyter from '$lib/images/devicon_jupyter-wordmark.png';
	import mongodb from '$lib/images/devicon_mongodb-wordmark.png';
	import typescript from '$lib/images/devicon_typescript.png';
	import js from '$lib/images/vscode-icons_file-type-js-official.png';
	

	const skillset = [
		{
			image: ImagePlaceholder,
			text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com',
			title: 'Product design',

		},
		{
			image: ImagePlaceholder,
			text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com',
			title: 'Art direction',

		},
		{
			image: ImagePlaceholder,
			text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com',
			title: 'Visual design',

		},
		{
			image: ImagePlaceholder,
			text: 'This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com',
			title: 'Visual design',

		},



	];
</script>

<div class="h-full w-full ">
    <div class="p-5 mb-12">
		<div class="m-12 ">
			<div class="flex justify-center text-3xl font-semibold text-[#FF64B4] mt-5 mb-[5rem] ">Projects</div>
			<div class="m-12 grid grid-cols-3 gap-12">
				{#each skillset as skills}
				<Card
					CardData={{
						image: skills.image,
						title: skills.title,
						text: skills.text,
				  
					}}
				/>
			{/each}
	
			</div>
		</div>

    </div>
    <div class="flex h-20">
		<div class=" mx-[8rem] flex h-full w-full items-center justify-evenly space-x-12 border-y border-gray-300">
			<img class=" h-auto w-10 max-w-full object-contain" src={typescript} alt="behance" />
			<img class=" h-auto w-11 max-w-full object-contain" src={js} alt="Google" />
			<img class=" h-auto w-[4rem] max-w-full object-contain" src={mongodb} alt="apple" />
			<img class=" h-auto w-[3rem] max-w-full object-contain" src={dotnet} alt="Dribble" />
			<img class=" h-auto w-[3rem] object-contain" src={jupyter} alt="awwwarrds" />
		</div>
	</div>

</div>