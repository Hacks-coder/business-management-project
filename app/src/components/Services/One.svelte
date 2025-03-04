<script lang="ts">
    import IconArrowRight from '~icons/mdi/arrow-right';
    import IconChartBar from '~icons/mdi/chart-bar';
    import IconAccountCircle from '~icons/mdi/account-circle';
	import Caption from "../resuable/Caption.svelte";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
    const servicesAnalysis = [
        { icon: IconArrowRight, service: "Redireation Tools" },
        { icon: IconChartBar, service: "Powerful Statistics" },
        { icon: IconAccountCircle, service: "Beautiful Profile" }
    ]

</script>
<section class="@container mt-30 ">
    <div class="grid place-items-center gap-10 @4xl:grid-cols-2 @5xl:px-4 @6xl:px-30 @7xl:px-40" >
        <div class="bg-purple size-72 flex justify-center items-center rounded-2xl  @xl:size-100 @3xl:size-130">
            <img src="/services/finance.png" alt="">
        </div>
        <div class="w-80 flex flex-col @2xl:w-100 gap-2 @4xl:w-130">
            <Caption />
            <Title text = "Business Process" />
            <Small text = "We Streamline your business processes, ensuring efficiency, productivity, and growth." />
            {#each servicesAnalysis as {icon, service}}
                <div class="flex gap-2">
                    <svelte:component this={icon} class="text-md text-blue @3xl:text-2xl"/>
                    <Small text = {service} />
                </div>
            {/each}
        </div>
    </div>
</section>