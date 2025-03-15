<script lang="ts">
    import IconFolderText from '~icons/mdi/folder-text';
    import IconChartLine from '~icons/mdi/chart-line';
    import IconPill from '~icons/mdi/pill';

    import Small from "../Texts/Small.svelte";
    import Title from "../Texts/Title.svelte";
	import Caption from '../staticDirs/Caption.svelte';

    const servicesAnalysis = [
        { icon: IconFolderText, service: "Electronic Health Records (EHR)" },
        { icon: IconChartLine, service: "Doctor Performance Analytics" },
        { icon: IconPill, service: "Prescription Management System" }
    ];
</script>

<section class="@container mt-30 ">
    <div class="flex flex-col items-center justify-center gap-10 @4xl:flex-row @4xl:justify-center @4xl:gap-30 @5xl:px-4 @6xl:px-30 @7xl:px-40" >
        <div class="size-72 flex justify-center items-center rounded-2xl  @xl:size-100 @3xl:size-130">
            <img src="/services/img3.png" alt="">
        </div>
        <div class="w-80 flex flex-col @2xl:w-100 gap-2 @4xl:w-130">
            <Caption />
            <Title text="Business Process" />
            <Small text="We enhance healthcare workflows by managing prescriptions, tracking health records, and analyzing staff performance." />
            {#each servicesAnalysis as {icon, service}}
                <div class="flex gap-2">
                    <svelte:component this={icon} class="text-md text-blue @3xl:text-2xl"/>
                    <Small text={service} />
                </div>
            {/each}
        </div>
    </div>
</section>
