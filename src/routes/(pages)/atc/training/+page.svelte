<script lang="ts">
	import { Hammer } from 'lucide-svelte';

	import bgImage from '$lib/assets/images/bg.png';
</script>

<main class="flex flex-col">
	<section class="h-screen bg-cover bg-center bg-no-repeat" style="background-image: url({bgImage});">
		<div class="h-full bg-black/50">
			<div class="container flex h-full flex-col items-center justify-center">
				<div class="flex flex-col items-center gap-4 text-2xl font-bold text-secondary md:text-4xl">
					<Hammer size={60} /> Page Under Construction
				</div>
			</div>
		</div>

		<div class="relative">
			<div class="absolute bottom-0 h-20 w-full bg-gradient-to-t from-base-300"></div>
		</div>
	</section>
</main>
