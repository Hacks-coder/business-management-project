<script>

	import Caption from "../resuable/Caption.svelte";
	import Small from "../Texts/Small.svelte";

</script>


<div class="@container mt-30 p-2">
    <div class="grid place-items-center gap-10 @3xl:grid-cols-2">
        <div>
            <img src="/others/doc.png " width="400" alt="">
        </div>
        <div>
            <div class="space-y-2">
                <Caption />
                <p class="text-2xl text-white  font-bold @xl:text-3xl @2xl:text-4xl @4xl:text-7xl">Divide each idea into small, manageable steps.</p>
                <Small text = "Dividing each idea into small, manageable steps means breaking a complex goal into clear, bite-sized tasks that you can tackle one at a time." />
            </div>
            <div class="flex gap-1 bg-white rounded-full px-1 py-2 justify-between mt-5 w-90 @2xl:w-120">
                <input type="email" placeholder="Subscribe" class="flex-1 outline-none"><button class="px-5 py-2 rounded-full bg-darkPurple text-white">Email</button>
            </div>
        </div>
    </div>
</div>