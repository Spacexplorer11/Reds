{#snippet cardGroup()}
	{#each Array(4) as _}
		<button type="button">
			<img alt="back of a card" src="/images/cards/cardback.webp" />
		</button>
	{/each}
{/snippet}

<div class="@container/top mb-[15vh] ml-[40%] grid max-w-[20%] grid-cols-2 gap-1.25">
	{@render cardGroup()}
</div>

<div class="@container/middle grid grid-cols-2">
	<div class="@container/left ml-[10%] grid max-w-[40%] rotate-90 grid-cols-2 gap-1.25">
		{@render cardGroup()}
	</div>
	<div class="@container/right ml-[50%] grid max-w-[40%] -rotate-90 grid-cols-2 gap-1.25">
		{@render cardGroup()}
	</div>
</div>

<div class="@container/bottom mt-[15vh] ml-[40%] grid max-w-[20%] grid-cols-2 gap-1.25">
	{@render cardGroup()}
</div>
