<script lang="ts">
	let { children } = $props();
	const authBG = "/auth/register.png"
</script>


<div class="@container">
	<div class="bg-white grid gap-5 @3xl:grid-cols-2 @3xl:gap-10">
		<div  class="flex flex-col  justify-center items-center w-full @3xl:h-screen @3xl:bg-blue" >
			<img src={authBG} alt="" class="size-50 @md:size-80 @xl:size-55 @3xl:size-100 @5xl:size-150">
		</div>
		<div class="w-full flex flex-col justify-center items-center">
			{@render children()}
		</div>
	</div>
</div>
