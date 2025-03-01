<script>
	import Medium from "../Texts/Medium.svelte";



</script>






<header class="@container p-5">
    <nav class="hidden @4xl:flex @4xl:justify-evenly">
        <Medium text = "Ochukonify" />
        <div class="flex gap-20">
            <a href="/home">Home</a>
            <a href="/services">Services</a>
            <a href="/contact">Contact</a>
        </div>
        <div class="space-x-3">
            <a href="/login">Login</a>
            <a href="/register" class="w-fit px-7 rounded-full py-2 bg-red text-white">Register</a>
        </div>
    </nav>
</header>