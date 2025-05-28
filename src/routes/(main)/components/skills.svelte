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
			text: 'This is a system for churces to digitally organize records for announcements,thanksgivings and church transfers, simplifying tasks for church secretaries, enhancing communication within the church community.',
			title: 'Announcement Management System',
			link: "https://atp-frontend.onrender.com/ "

		},
		{
			image: ImagePlaceholder,
			text: 'This is a web scraper to extract data from Amazon based on user-selected categories and departments, presenting products to enhance the shopping experience by providing a curated list of items.',
			title: 'Scrapitos',
			link: "https://github.com/Yaa-Henewaa/scrapitos "

		},
		{
			image: ImagePlaceholder,
			text: 'This is a reusable image upload service using RabbitMQ and Cloudinary, designed to handle image uploads efficiently and securely, providing a reliable solution for applications requiring image storage and retrieval.',
			title: 'Image-Upload Service ',
			link: "https://github.com/Yaa-Henewaa/Image-Upload-Service"

		},




	];
</script>

<div class="h-full w-full">
    <div class="p-4 sm:p-5 mb-8 sm:mb-12">
        <div class="px-4 mt-4">
            <div class="flex justify-center text-2xl sm:text-3xl font-semibold text-[#FF64B4] mt-4 sm:mt-5 mb-6 sm:mb-[5rem]">
                Projects
            </div>
            
            <!-- Changed grid to be responsive -->
            <div class="mx-4 sm:m-12 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 sm:gap-8 lg:gap-12">
                {#each skillset as skills}
                    <Card
                        CardData={{
                            image: skills.image,
                            title: skills.title,
                            text: skills.text,
                            link: skills.link
                        }}
                    />
                {/each}
            </div>
        </div>
    </div>

    <!-- Technology stack section -->
    <div class="flex h-auto sm:h-20 py-6 sm:py-0">
        <div class="mx-4 sm:mx-[4rem] lg:mx-[8rem] flex flex-wrap sm:flex-nowrap w-full items-center justify-center sm:justify-evenly gap-6 sm:gap-8 lg:gap-12 border-y border-gray-300 py-4 sm:py-0">
            <img class="h-8 sm:h-10 w-auto object-contain" src={typescript} alt="TypeScript" />
            <img class="h-8 sm:h-10 w-auto object-contain" src={js} alt="JavaScript" />
            <img class="h-8 sm:h-12 w-auto object-contain" src={mongodb} alt="MongoDB" />
            <img class="h-8 sm:h-10 w-auto object-contain" src={dotnet} alt=".NET Core" />
            <img class="h-8 sm:h-10 w-auto object-contain" src={jupyter} alt="Jupyter" />
        </div>
    </div>
</div>