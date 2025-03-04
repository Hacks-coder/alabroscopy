<script>

	import Small from "../Texts/Small.svelte";
    const photo = '/others/hero.png'
</script>
<section class="@container mt-10">
    <div class="grid place-items-center gap-10 @3xl:grid-cols-2">
        <div class="text-center flex flex-col items-center gap-5    ">
            <p class="border-4 border-pink rounded-full pl-5 pr-5 text-md w-fit @md:text-2xl @xl:text-3xl">What’s New?</p>
            <p class="text-3xl font-big font-bold bg-clip-text text-transparent bg-[linear-gradient(to_right,_#5963FF_0%,_#5963FF_20%,_#C837AB_80%,_#C837AB_100%)] @md:text-4xl @2xl:text-5xl @4xl:text-6xl">Mental Health is Wealth</p>
            <div class="grid grid-cols-[5px_300px] gap-15">
                <div class="w-15 h-15 rounded-full bg-pink"></div>
                <Small text = "To live your life to the fullest we have provide a means where you can track your medical report." />
            </div>
        </div>
        <div style={`background-image: url(${photo})`} class="size-72 bg-cover bg-center @xl:size-100 @4xl:size-130 @5xl:size-150"></div>
    </div>
</section>