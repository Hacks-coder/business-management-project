<script>
	import Medium from "../Texts/Medium.svelte";


	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";

</script>
<footer class="@container mt-30 bg-darkPurple p-5 text-white flex flex-col gap-10 2xl:p-20">
    <div class="grid gap-10 @4xl:grid-cols-3 @4xl:place-items-center">
        <div class="space-y-5">
            <Title text = "Ochukonify" />
            <Small text  = "The web platform aims to enable free link shortener free from aids and you get to do mini task with no pricing attached to them. Sounds great right? Let’s do this." />
        </div>
        <div class="flex flex-col gap-3">
            <Title text = "Company" />
            <a href="/contact">Contact</a>
            <a href="/help-us">Help Us</a>
        </div>
        <div class="space-y-3">
            <Title text = "New Letter" />
            <Small text = "Get messages as a reminder" />
            <div class="rounded-full w-fit flex p-1 bg-white">
                <input type="email" class="outline-none text-darkPurple"> <button class="bg-darkPurple rounded-full px-5 py-1">Send</button>
            </div>
        </div>
    </div>
    <div>
        <hr class="mb-5">
        <div class="@4xl:flex @4xl:justify-between">
            <Small text = "Ochukonify 2025. All Rights Reserved" />
            <div class="flex gap-3 text-sm">
                <a href="/privacy">Privacy</a>
                <a href="terms">Terms</a>
                <a href="report">Report</a>
            </div>
        </div>
    </div>
</footer>