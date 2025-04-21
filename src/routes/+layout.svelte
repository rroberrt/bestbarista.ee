<script lang="ts">
	import '../app.css';

	let { children } = $props();
</script>

<div class="flex h-screen flex-col">
	<header class="bg-black p-1">
		<div class="flex items-center justify-center gap-x-2">
			<img src="/us.svg" alt="UNITED STATES OF AMERICA" class="h-3" />
			<p class="text-center text-[0.7rem] text-white">
				Not an official website of the United States government
			</p>
		</div>
	</header>

	<main class="grow">
		{@render children()}
	</main>

	<footer class="p-4">
		<p class="text-center text-xs text-neutral-600 uppercase">Made by Bobby Shmurda</p>
	</footer>
</div>
