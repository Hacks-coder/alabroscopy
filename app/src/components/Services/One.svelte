<script lang="ts">
    import IconViewDashboard from '~icons/mdi/view-dashboard';
    import IconStethoscope from '~icons/mdi/stethoscope';
    import IconFileDocument from '~icons/mdi/file-document';
	import Caption from '../staticDirs/Caption.svelte';
	import Title from '../Texts/Title.svelte';
	import Small from '../Texts/Small.svelte';
    const servicesAnalysis = [
        { icon: IconViewDashboard, service: "Comprehensive Patient Dashboard" }, 
        { icon: IconStethoscope, service: "Efficient Doctor Management" }, 
        { icon: IconFileDocument, service: "Secure Medical Record Handling" } 
    ];
</script>

<section class="@container mt-30 ">
    <div class="flex flex-col items-center justify-center gap-10 @4xl:flex-row @4xl:justify-center @4xl:gap-30 @5xl:px-4 @6xl:px-30 @7xl:px-40" >
        <div class=" size-72 flex justify-center items-center rounded-2xl  @xl:size-100 @3xl:size-130">
            <img src="/services/img1.png" alt="">
        </div>
        <div class="w-80 flex flex-col @2xl:w-100 gap-2 @4xl:w-130">
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
    </div>
</section>
