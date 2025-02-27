<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>


<div class="overflow-hidden">
	{@render children()}
</div>
