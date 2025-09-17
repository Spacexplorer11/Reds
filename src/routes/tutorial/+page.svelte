<script>
	import { ArrowBigLeft, ArrowBigRight, House } from '@lucide/svelte';
	import steps from '$lib/tutorial';
	let step = $state(1);
	let stepJSON = $derived(steps[step - 1]);
</script>

<div class="@container mx-auto flex flex-col p-4 text-center text-black">
	<a href="/" class="-top-2.5 left-0.5 max-w-fit"><House /></a>
	<h1 class="text-4xl md:text-5xl">Tutorial</h1>
	<h2 class="my-4 text-2xl md:text-3xl">Learn how to play Reds!</h2>
	<main class="@container/main flex flex-row justify-center gap-10">
		<button
			class="max-w-fit rounded-2xl bg-blue p-5 disabled:cursor-not-allowed disabled:bg-gray-700"
			onclick={() => {
				if (step > 1) step -= 1;
			}}
			disabled={step <= 1}
		>
			<ArrowBigLeft size="30" />
		</button>
		<div class="@container/step flex w-3/5 flex-col items-center rounded-2xl bg-salmon p-10">
			<h3 class="my-2 text-2xl whitespace-pre-wrap md:text-3xl">{stepJSON.title}</h3>
			<p class="my-4 text-xl whitespace-pre-wrap md:text-2xl">
				{stepJSON.content}
			</p>
		</div>
		<button
			class="max-width-fit rounded-2xl bg-blue p-5 disabled:cursor-not-allowed disabled:bg-gray-700"
			onclick={() => {
				if (step < steps.length) step += 1;
			}}
			disabled={step >= steps.length}
		>
			<ArrowBigRight size="30" />
		</button>
	</main>
</div>
