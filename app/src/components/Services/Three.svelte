<script lang="ts">
	import Caption from "../resuable/Caption.svelte";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
</script>
<section class="@container mt-10">
    <div class="flex flex-col items-center justify-center gap-10 @4xl:flex-row @4xl:justify-center @4xl:gap-30 @5xl:px-4 @6xl:px-30 @7xl:px-40" >
        <div class="bg-beize  size-72 rounded-2xl @xl:size-100 @3xl:size-130">
            <img src="/services/bank.png" alt="">
        </div>
        <div class="w-80 flex flex-col  @2xl:w-100 gap-2 @4xl:w-130">
            <Caption />
            <Title text = "Financial Negotiations" />
            <Small text = "We navigate complex financial negotiations, securing the best deals and maximizing your returns" />
        </div>
    </div>
</section>