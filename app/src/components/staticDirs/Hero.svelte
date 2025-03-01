<script>

	import Caption from "../resuable/Caption.svelte";
	import Small from "../Texts/Small.svelte";

</script>


<div class="@container mt-30">
    <div class="grid place-items-center @3xl:grid-cols-2">
        <div>
            <img src="/others/doc.png " width="400" alt="">
        </div>
        <div>
            <div>
                <Caption />
                <p class="text-2xl font-bold">Divide each idea into small, manageable steps.</p>
                <Small text = "Dividing each idea into small, manageable steps means breaking a complex goal into clear, bite-sized tasks that you can tackle one at a time, making progress easier to track and the overall process less overwhelming." />
            </div>
            <div></div>
        </div>
    </div>
</div>