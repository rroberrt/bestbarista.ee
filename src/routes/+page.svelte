<script lang="ts">
	const wallets: { ccy: string; address: string }[] = [
		{ ccy: 'BTC', address: 'bc1qa9che390frvlkqs8md3jz9ygr3jaav60qx8fng' },
		{ ccy: 'ETH', address: '0x8aF20cFf2f3819943CAE6669416D1C6327e66abA' },
		{ ccy: 'SOL', address: 'Gmovjo9ixS2NGbL3E8cGcsNypCD1UvgfnA4QP4kyQMVW' },
		{ ccy: 'LTC', address: 'ltc1qtmerhg3rvw2z6dsyh8rqvq4j5zwcg57zplp7cx' },
		{ ccy: 'DOGE', address: 'DC9GkpG49whco53yr4s1ZPnjcKNVegAGLa' }
	];
</script>

<section class="flex h-full">
	<div class="container m-auto space-y-2 overflow-auto text-sm">
		<div class="mx-auto w-fit space-y-4 sm:space-y-2">
			{#each wallets as { ccy, address }, i (i)}
				<div class="flex flex-col gap-x-4 font-mono sm:flex-row sm:items-center">
					<p class="shrink-0 px-2 font-semibold sm:basis-10 sm:px-0">{ccy}</p>
					<p class="rounded bg-neutral-100 px-2 py-1">{address}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
