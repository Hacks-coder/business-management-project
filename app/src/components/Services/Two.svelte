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
<section class="@container mt-30 ">
    <div class="grid place-items-center gap-30 @4xl:grid-cols-2 @5xl:px-4 @6xl:px-30 @7xl:px-40" >
        <div class="w-80 flex flex-col @2xl:w-100 gap-2 @4xl:w-130">
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
        <div class="bg-skyBlue size-72 rounded-2xl shadow-sm shadow-gray-600 @xl:size-100 @3xl:size-130">
            <img src="/services/partnership.png" alt="">
        </div>
    </div>
</section>