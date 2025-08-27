<script lang="ts">
	import type { PageProps } from './$types';

	import { CalendarHeart } from 'lucide-svelte';

	import Events from '$lib/components/Events.svelte';

	import bgImage from '$lib/assets/images/bg.png';

	let { data }: PageProps = $props();
</script>

<main class="flex flex-col">
	<section class="h-[40vh] bg-cover bg-center bg-no-repeat" style="background-image: url({bgImage});">
		<div class="h-full bg-black/50">
			<div class="container flex h-full flex-col items-center justify-center">
				<div class="flex items-center gap-2 text-2xl font-bold text-secondary md:text-4xl">
					<CalendarHeart size={36} /> Events
				</div>
			</div>
		</div>

		<div class="relative">
			<div class="absolute bottom-0 h-20 w-full bg-gradient-to-t from-base-300"></div>
		</div>
	</section>

	<section class="bg-base-300 py-10">
		<div class="container flex min-h-[40vh] flex-col items-center justify-center">
			{#if data.events}
				<Events events={data.events} />
			{:else}
				There are currently no upcoming events.
			{/if}
		</div>
	</section>
</main>
