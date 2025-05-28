<script>
    import twitter from '$lib/images/fa6-brands_square-x-twitter.png';
    import linkedin from '$lib/images/fa6-brands_linkedin.png';
    import github from '$lib/images/fa6-brands_github.png';
</script>

<div class="h-full w-full ">
    <div class=" flex  p-5 ">
        <div class="m-12 items-start flex w-full  justify-evenly border-t border-gray-200">
            <div class="space-y-5 py-10 mt-10">
                <p class="font-semibold text-2xl text-[#FF64B4]">Let's work together</p>
                <p class="w-[30rem] text-lg">I'm open to freelance opportunities and would love to collaborate! If you have any requests or questions, feel free to reach out—I'm here to help!</p>
                <div class="flex h-auto w-8 space-x-4 max-w-full object-contain ">
                    <img src={linkedin} alt="">
                    <img src={github} alt="">
                    <img src={twitter} alt="">
                    
                </div>
            </div>
            <div class="py-10 mt-8 w-[27rem] ml-8 space-y-5  ">
                <input class=" border-none w-full rounded-md bg-gray-100 py-2 pl-4 pr-4" type="text" placeholder="Name">
                <input class=" border-none w-full rounded-md bg-gray-100 py-2 pl-4 pr-4" type="email" placeholder="Email">
                <input class="h-[10rem] border-none rounded-md w-full bg-gray-100 py-2 pl-4 pb-[8rem] " type="text" placeholder="Type your message here">
                <button class="bg-[#FF64B4] rounded-lg text-lg text-white text-center p-3 w-[7rem]">Submit</button>
            </div>
        </div>
    </div>
</div>