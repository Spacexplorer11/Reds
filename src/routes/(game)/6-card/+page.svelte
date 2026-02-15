{#snippet cardGroup()}
	{#each Array(6) as _}
		<button type="button">
			<img alt="back of a card" src="/images/cards/cardback.webp" />
		</button>
	{/each}
{/snippet}

<div class="@container/top mb-[15vh] ml-[35%] grid max-w-[30%] grid-cols-3 gap-1.25">
	{@render cardGroup()}
</div>

<div class="@container/middle grid grid-cols-2">
	<div class="@container/left grid max-w-[50%] rotate-90 grid-cols-3 gap-1.25">
		{@render cardGroup()}
	</div>
	<div class="@container/right ml-[50%] grid max-w-[50%] rotate-270 grid-cols-3 gap-1.25">
		{@render cardGroup()}
	</div>
</div>

<div class="@container/bottom mt-[15vh] ml-[35%] grid max-w-[30%] grid-cols-3 gap-1.25">
	{@render cardGroup()}
</div>
