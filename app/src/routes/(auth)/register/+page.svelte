<script>
	import Fill from '../../../components/Buttons/Fill.svelte';
	import Title from '../../../components/Texts/Title.svelte';
	import Small from './../../../components/Texts/Small.svelte';
</script>

<div class="text-center space-y-3">
    <Title text = "Registration System" />
    <Small text = "Fill in all the fields below." /> 
</div>


<form action="" class="flex flex-col gap-5 mt-10 @3xl:text-2xl">
    <div class="flex flex-col gap-2">
        <label for="" class="font-krona font-bold text-md">Email</label>
        <input type="text" placeholder="Email" class="w-80 h-10 bg-skyBlue focus:outline-blue @4xl:w-130 @4xl:h-15">
    </div>
    <div class="flex flex-col gap-2">
        <label for="" class="font-krona font-bold text-md">Password</label>
        <input type="text" placeholder="Email" class="w-80 h-10 bg-skyBlue focus:outline-blue @4xl:w-130 @4xl:h-15">
    </div>
    <div class="flex justify-between text-blue">
        <div class="flex gap-2"><input type="checkbox"><Small text = "Remember Me?" /></div>
        <Small text = "forgot password?" />
    </div>
    <Fill text="Register" />
    <div class="flex justify-between">
        <Small text = "I already have an account." /> <a href="/login" class="text-blue text-sm font-main" >Sign-in</a>
    </div>
</form>