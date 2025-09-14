<script>
</script>

<div class="@container mx-auto flex flex-col p-4 text-center text-black">
	<h1 class="text-4xl md:text-5xl">Welcome to Reds!</h1>
	<h2 class="my-4 text-2xl md:text-3xl">Please select a button below</h2>
	<div class="@container/buttons w-full space-y-6">
		<div class="@container/4-cards mx-auto flex flex-col items-center">
			<button
				id="tutorial"
				class="my-2 min-w-[80%] rounded-2xl bg-salmon py-14 text-2xl hover:-translate-y-2 hover:scale-[1.03] hover:shadow-2xl md:text-3xl"
				onclick={(window.location.href = '/tutorial')}>Tutorial</button
			>
			<p class="text-xl md:text-2xl">Don't know how to play?</p>
		</div>
		<div class="@container/4-cards mx-auto flex flex-col items-center">
			<button
				id="4-cards"
				class="my-2 min-w-[80%] rounded-2xl bg-blue py-14 text-2xl hover:-translate-y-2 hover:scale-[1.03] hover:shadow-2xl md:text-3xl"
				>4 cards</button
			>
			<p class="text-xl md:text-2xl">You will be able to look at the first <b>2</b> cards</p>
		</div>
		<div class="@container/6-cards mx-auto flex flex-col items-center">
			<button
				id="6-cards"
				class="my-2 min-w-[80%] rounded-2xl bg-green py-14 text-2xl hover:-translate-y-2 hover:scale-[1.03] hover:shadow-2xl md:text-3xl"
				>6 cards</button
			>
			<p class="text-xl md:text-2xl">You will be able to look at the first <b>3</b> cards</p>
		</div>
	</div>
</div>
