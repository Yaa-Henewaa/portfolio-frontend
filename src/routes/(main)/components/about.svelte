<script>
    import About from '$lib/images/doodles mixed round.png';
    import About2 from '$lib/images/Group 2346 (1).png';
</script>

<div class="h-full w-full">
    <div class="m-auto mx-auto flex max-w-screen-2xl p-4 sm:p-5">
        <div class="mx-4 lg:m-12 flex flex-col-reverse lg:flex-row w-full items-center justify-between gap-8">
            <!-- Text Section -->
            <div class="w-full space-y-4 py-4 sm:py-6 lg:py-8 lg:w-3/5">
                <p class="text-2xl sm:text-3xl lg:text-4xl pl-1 font-semibold">Hi! I'm</p>
                <p class="text-4xl sm:text-5xl lg:text-7xl font-semibold text-[#FF64B4]">Maame Henewaa</p>
                <div class="w-full pl-1 text-lg sm:text-xl">
                    Software Engineer based in Accra, Ghana 🇬🇭
                </div>
            </div>

            <!-- Image Section -->
            <div class="w-full lg:w-2/5 relative max-w-xs sm:max-w-sm lg:max-w-md mx-auto">
                <img 
                    class="h-auto w-full object-contain" 
                    src={About} 
                    alt="Decorative background illustration"
                />
                <img 
                    src={About2} 
                    alt="Profile overlay" 
                    class="absolute top-4 left-4 sm:top-5 sm:left-5 lg:top-7 lg:left-7 w-full h-auto"
                >
            </div>
        </div>
    </div>
</div>
