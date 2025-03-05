<script>
	import Small from "../Texts/Small.svelte";

    const testimonies = [
    {
        src: "/testimonies/img3.jpg",
        title: "A Healthier, Happier You",
        description: "Managing my health has never been easier! This platform provides seamless access to medical services, ensuring I stay on top of my well-being."
    },
    {
        src: "/testimonies/img2.jpg",
        title: "Reliable and Life-Changing",
        description: "This website has transformed the way I handle medical appointments and records. The efficiency and support are truly outstanding!"
    },
    {
        src: "/testimonies/img1.jpg",
        title: "Your Health, Our Priority",
        description: "With this platform, I feel more in control of my health than ever before. The convenience and care it offers are simply unmatched!"
    }
]
    
</script>


<section>
    <div>
        <div class="flex flex-col items-center px-5 @md:px-10 @xl:px-15  gap-10 @3xl:px-5 @3xl:flex-row @3xl:px-20 @5xl:gap-15">
           {#each testimonies as {src, title, description}}
                <div class="flex flex-col items-center gap-2">
                    <div class="overflow-hidden w-60 rounded-2xl h-fit @md:w-80 @3xl:w-60 @4xl:w-80">
                        <img {src} alt="">
                    </div>
                    <p class="text-purple font-bold text-xl @xl:text-2xl">{title}</p>
                    <Small text = {description} />
                </div>
           {/each}
        </div>
    </div>
</section>