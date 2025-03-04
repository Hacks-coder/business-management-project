<script>
	import Fill from '../../../components/Buttons/Fill.svelte';
	import Title from '../../../components/Texts/Title.svelte';
	import Small from '../../../components/Texts/Small.svelte';
</script>

<div class="text-center space-y-3">
    <Title text = "Registration System" />
    <Small text = "Fill in all the fields below." /> 
</div>


<form action="" class="flex flex-col gap-5 mt-10 @3xl:text-2xl">
    <div class="flex flex-col gap-2">
        <label for="" class="font-krona font-bold text-md">Message Title</label>
        <input type="text" placeholder="Title" class="w-80 h-10 bg-white shadow-md outline-1 outline-blue focus:outline-blue @4xl:w-110 @4xl:h-15">
    </div>
    <div class="flex flex-col gap-2">
        <label for="" class="font-krona font-bold text-md">Message Body</label>
        <textarea placeholder="Enter message here..." class="w-80 h-32 shadow-md outline-1 outline-blue focus:outline-blue @4xl:w-110 @4xl:h-60"></textarea>
    </div>
    <Fill text="Send Message" />
</form>