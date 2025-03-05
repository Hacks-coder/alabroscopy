<script>
	import Small from "../Texts/Small.svelte";

    const testimonies = [
        {
            src: "/testimonies/img3.jpg",
            title: "Bring your inner peace",
            description: "This is the best cite to manage your health"
        },
        {
            src: "/testimonies/img2.jpg",
            title: "Come and manage with us",
            description: "This is the best cite to manage your health"
        },
        {
            src: "/testimonies/img1.jpg",
            title: "Stabilise your heath with us",
            description: "This is the best cite to manage your health"
        }
    ]
    
    
</script>


<section>
    <div>
        <div class="flex flex-col gap-10 @3xl:flex-row @5xl:gap-15">
           {#each testimonies as {src, title, description}}
                <div class="space-y-3">
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