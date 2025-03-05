<script>
	import Testimonies from './../Cards/Testimonies.svelte';
	import Small from "../Texts/Small.svelte";


	import Title from "../Texts/Title.svelte";

</script>
<section class="@container text-center mt-20">
    <div class="flex flex-col gap-2 items-center">
        <p class="border-4 border-pink px-10 py-2 rounded-full">Testimonies</p>
        <div>
            <Title text = "Discover Your Inner Peace" />
            <Small text = "Real Stories, Real Impact: Hear from Those Who Trust Us" />
        </div>
        <div class="mt-10">
            <Testimonies />
        </div>
    </div>
    
</section>