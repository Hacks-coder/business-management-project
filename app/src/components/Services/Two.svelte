<script lang="ts">
    import IconMicrophone from '~icons/mdi/microphone';    
    import IconNewspaper from '~icons/mdi/newspaper';          
    import IconBriefcase from '~icons/mdi/briefcase';
	import Caption from "../resuable/Caption.svelte";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
    const servicesAnalysis = [
    { icon: IconMicrophone, service: "Public Speaking" },
    { icon: IconNewspaper, service: "Rich Articles" },
    { icon: IconBriefcase, service: "Business Planning" }
  ];

</script>
<section class="@container mt-10 ">
    <div class="flex flex-col items-center justify-center  gap-10 @4xl:flex-row @4xl:justify-center @4xl:gap-30 @5xl:px-4 @6xl:px-30 @7xl:px-40" >
        <div class="w-80 order-1 flex flex-col @2xl:w-100 gap-2 @4xl:w-130 @4xl:order-0">
            <Caption />
            <Title text = "Strategic Partnerships" />
            <Small text = "We foster strategic partnerships, connecting you  with the right people, resources, and opportunities." />
            {#each servicesAnalysis as {icon, service}}
                <div class="flex gap-2">
                    <svelte:component this={icon} class="text-md text-blue @3xl:text-2xl"/>
                    <Small text = {service} />
                </div>
            {/each}
        </div>
        <div class="bg-skyBlue size-72 rounded-2xl @xl:size-100 @3xl:size-130">
            <img src="/services/partnership.png" alt="">
        </div>
    </div>
</section>