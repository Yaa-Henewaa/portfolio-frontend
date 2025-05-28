<script lang="ts">

	type CardDataProps = {
		image: string;
		title: string;
		text: string;
	};
	export let CardData: CardDataProps;
</script>


<div class="flex flex-col col-span-1 justify-center items-center gap-4">
    <div class="w-[100px] ">
        <img src={CardData.image} alt="">
    </div>
    <p class="text-xl font-semibold text-[#FF64B4]"> {CardData.title}</p>
    <p class="text-lg mx-3 w-[25rem]">{CardData.text}</p>
</div>