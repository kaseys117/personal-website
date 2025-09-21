<script lang="ts">
	import '../app.css';
	import Navbar from '$lib/navbar.svelte'


	let { children } = $props();
</script>

<div class="mx-auto flex min-h-screen flex-col max-w-[68rem] px-2 pt-2">
	<Navbar/>
	<main class='flex-1 md:py-10 flex flex-col'>
		{@render children()}
	</main>
</div>