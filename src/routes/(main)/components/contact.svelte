<script>
    import emailjs from '@emailjs/browser';
    import { onMount } from 'svelte';
    import twitter from '$lib/images/fa6-brands_square-x-twitter.png';
    import linkedin from '$lib/images/fa6-brands_linkedin.png';
    import github from '$lib/images/fa6-brands_github.png';

    
    let name = '';
    let email = '';
    let message = '';
    let loading = false;

    const sendEmail = async () => {
        loading = true;
        try {
            await emailjs.send(
                'service_n2umur7', // Replace with your EmailJS service ID
                'template_lt6gq9l', // Replace with your template ID
                {
                    from_name: name,
                    from_email: email,
                    message: message,
                    to_name: 'maameyaahenewaa2001@gmail.com', // Replace with your name
                },
                'g9kKqIyZ9D3TzY2xD' // Replace with your public key
            );
            alert('Message sent successfully!');
            // Clear form
            name = '';
            email = '';
            message = '';
        } catch (error) {
            console.error('Error:', error);
            alert('Failed to send message. Please try again.');
        }
        loading = false;
    };

    // Add your social media URLs
    const socialLinks = {
        linkedin: "https://www.linkedin.com/in/yaahenewaa/",
        github: "https://github.com/Yaa-Henewaa",
       
    };
</script>

<div class="min-h-screen w-full px-4 sm:px-6 lg:px-8">
    <div class="flex flex-col p-4 sm:p-5">
        <div class="mx-4 lg:m-12 flex flex-col lg:flex-row w-full items-start justify-between gap-8 border-t border-gray-200">
            <!-- Left section - Text and Social Links -->
            <div class="w-full lg:w-1/2 space-y-5 py-6 lg:py-10">
                <p class="font-semibold text-xl sm:text-2xl text-[#FF64B4]">Let's work together</p>
                <p class="w-full lg:w-[30rem] text-base sm:text-lg">
                    I'm open to freelance opportunities and would love to collaborate! If you have any requests or questions, feel free to reach out—I'm here to help!
                </p>
                <div class="flex gap-4 items-center">
                    <a href={socialLinks.linkedin} target="_blank" rel="noopener noreferrer">
                        <img src={linkedin} alt="LinkedIn Profile" class="w-6 h-6 sm:w-8 sm:h-8 hover:opacity-80 transition-opacity">
                    </a>
                    <a href={socialLinks.github} target="_blank" rel="noopener noreferrer">
                        <img src={github} alt="GitHub Profile" class="w-6 h-6 sm:w-8 sm:h-8 hover:opacity-80 transition-opacity">
                    </a>
                </div>
            </div>

            <!-- Right section - Contact Form -->
            <div class="w-full lg:w-1/2 space-y-4 sm:space-y-5 py-6 lg:py-10">
                <div class="max-w-md mx-auto lg:mx-0">
                    <input 
                        bind:value={name}
                        class="border-none w-full rounded-md bg-gray-100 py-2 px-4 text-base sm:text-lg" 
                        type="text" 
                        placeholder="Name"
                    >
                    <input 
                        bind:value={email}
                        class="border-none w-full rounded-md bg-gray-100 py-2 px-4 text-base sm:text-lg mt-4" 
                        type="email" 
                        placeholder="Email"
                    >
                    <textarea 
                        bind:value={message}
                        class="h-[8rem] sm:h-[10rem] border-none rounded-md w-full bg-gray-100 py-2 px-4 text-base sm:text-lg mt-4" 
                        placeholder="Type your message here"
                    ></textarea>
                    <button 
                        on:click={sendEmail} 
                        class="bg-[#FF64B4] rounded-lg text-base sm:text-lg text-white text-center p-2 sm:p-3 w-[6rem] sm:w-[7rem] hover:bg-opacity-90 transition-colors mt-4"
                        disabled={loading}
                    >
                        {loading ? 'Sending...' : 'Submit'}
                    </button>
                </div>
            </div>
        </div>
    </div>
</div>