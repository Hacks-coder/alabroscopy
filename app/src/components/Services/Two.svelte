<script lang="ts">
    import IconAccountMultiple from '~icons/mdi/account-multiple';
    import IconCalendarCheck from '~icons/mdi/calendar-check';
    import IconFileDocumentOutline from '~icons/mdi/file-document-outline';
    
    import Small from "../Texts/Small.svelte";
    import Title from "../Texts/Title.svelte";
	import Caption from '../staticDirs/Caption.svelte';

    const servicesAnalysis = [
        { icon: IconAccountMultiple, service: "Comprehensive Patient Management" },
        { icon: IconCalendarCheck, service: "Smart Appointment Scheduling" },
        { icon: IconFileDocumentOutline, service: "Billing & Medical Invoicing" }
    ];
</script>

<section class="@container mt-30 ">
    <div class="flex flex-col items-center justify-center gap-10 @4xl:flex-row @4xl:justify-center @4xl:gap-30 @5xl:px-4 @6xl:px-30 @7xl:px-40" >
        <div class="w-80 flex order-1 flex-col @2xl:w-100 gap-2 @4xl:w-130 @4xl:order-0">
            <Caption />
            <Title text="Business Process" />
            <Small text="We streamline your healthcare operations, boosting efficiency, accuracy, and patient care outcomes." />
            {#each servicesAnalysis as {icon, service}}
                <div class="flex gap-2">
                    <svelte:component this={icon} class="text-md text-blue @3xl:text-2xl"/>
                    <Small text={service} />
                </div>
            {/each}
        </div>
        <div class=" size-72 flex justify-center items-center rounded-2xl  @xl:size-100 @3xl:size-130">
            <img src="/services/img2.png" alt="">
        </div>
    </div>
</section>
