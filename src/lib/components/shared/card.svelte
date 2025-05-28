<script lang="ts">
	import { Link } from "lucide-svelte";


	type CardDataProps = {
		image: string;
		title: string;
		text: string;
		link?: string;
	};
	export let CardData: CardDataProps;
</script>


<div class="flex flex-col col-span-1 justify-center items-center gap-4">
    <div class="w-[100px] ">
        <img src={CardData.image} alt="">
    </div>
    <a href={CardData.link} target="_blank"><p class="text-xl font-semibold text-[#FF64B4]"> {CardData.title}</p> </a>
    <p class="text-lg w-[25rem] text-center">{CardData.text}</p>
</div>