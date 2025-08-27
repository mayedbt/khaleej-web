<script lang="ts">
	import { ArrowDown } from 'lucide-svelte';

	import bgImage from '$lib/assets/images/bg.png';
</script>

<main class="flex flex-col">
	<section class="h-screen bg-cover bg-center bg-no-repeat" style="background-image: url({bgImage});">
		<div class="h-full bg-black/50">
			<div class="container flex h-full flex-col items-center justify-center">
				<h1 class="text-center text-4xl md:text-6xl">Ready to embark on an unforgettable journey?</h1>
			</div>

			<div class="relative bottom-60">
				<ArrowDown size={20} class="m-auto h-10 w-10 animate-bounce text-secondary" />
			</div>
		</div>

		<div class="relative">
			<div class="absolute bottom-0 h-20 w-full bg-gradient-to-t from-base-300"></div>
		</div>
	</section>

	<section class="bg-base-300 py-10">
		<div class="container flex min-h-[40vh] flex-col items-center">
			<div class="hero">
				<div class="hero-content flex-col gap-8 lg:flex-row">
					<enhanced:img src="../../../lib/assets/images/bg.png" alt="Join Image" class="w-[28rem] rounded-lg shadow-2xl" />

					<div class="flex flex-col gap-6">
						<p class="max-w-md">
							Join a world full of opportunities and experiences, filled with events and activities. Whether you're a seasoned pilot or
							a veteran controller, the skies of Bahrain and Kuwait are open for you.
						</p>

						<!-- Disabled for now due to Discord integration -->
						<button class="btn btn-disabled">Get Started</button>
					</div>
				</div>
			</div>
		</div>
	</section>
</main>

<style lang="postcss">
</style>
