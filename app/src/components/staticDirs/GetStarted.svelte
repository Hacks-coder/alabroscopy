<script>
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
    const nurse = "/others/doForU.png"
</script>

<section class="@container mt-20 pr-10 pl-10">
    <div class="grid place-items-center text-center gap-10 @3xl:grid-cols-2">
        <div style={`background-image: url(${nurse})`} class="bg-cover bg-center size-72 @xl:size-80 @2xl:size-110 @4xl:size-150"></div>
        <div class="flex flex-col gap-5 items-center">
            <Title text = "How can we help you?" />
            <Small text = "We collaborate with world-class experts to develop innovative, human-centered tools and services that drive sustainable growth and improve healthcare outcomes. Our data-driven approach ensures that every decision is carefully tailored to enhance your well-being, empowering you with smarter, more effective solutions. By integrating advanced technology with expert insights." />
        </div>
    </div>
</section>