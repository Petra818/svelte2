<script>
	import { assets } from '$app/paths';

	import { Aperture, Menu } from '@lucide/svelte';

	import '../app.css';
	import { page } from '$app/state';
	import { render } from 'svelte/server';
	import Footer from '$lib/components/Footer.svelte';
	import { afterNavigate } from '$app/navigation';

	let { children } = $props();
	let mobileNavOpen = $state(false);

	afterNavigate(() => {
		mobileNavOpen = false;
	});
</script>

<header class="  h-15 flex justify-center border-b-2 bg-gray-400">
	<!-- MOBILE -->
	<button
		class=""
		onclick={() => {
			mobileNavOpen = !mobileNavOpen;
		}}><Menu /></button
	>

	<section
		class=" absolute left-0 right-0 flex-col lg:hidden {mobileNavOpen
			? 'top-0.5 flex duration-1000'
			: 'duration-2000 top-[-1000px]'}"
	>
		<div
			class=" gabarito-uniquifier fixed left-0 mt-14 w-full border-b-2 border-t-2 border-t-gray-500 bg-gray-300 p-6"
		>
			<div class=" flex items-center justify-center">
				<a class="rounded-4xl p-3 hover:bg-gray-500" href="/">Domov</a>
				<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/aboutme">O nás</a>
				<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/websites">Stránky</a>
			</div>
			<div class="flex items-center justify-center">
				<Aperture class="size-10 stroke-2 text-black " />
			</div>
			<div class=" flex items-center justify-center">
				<a href="/projects" class=" rounded-4xl p-3 hover:bg-gray-500">Projekty</a>
				<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/skills">Zručnosti</a>
				<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/contact">Kontakt</a>
			</div>
		</div>
	</section>

	<section class="hidden lg:flex">
		<div class="gabarito-uniquifier space-x-7 p-3 text-2xl">
			<a class="rounded-4xl p-3 hover:bg-gray-500" href="/">Domov</a>
			<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/aboutme">O nás</a>
			<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/websites">Stránky</a>
		</div>
		<div class="p-2">
			<Aperture class="size-10 stroke-2 text-black" />
		</div>
		<div class="gabarito-uniquifier space-x-7 p-3 text-2xl">
			<a href="/projects" class=" rounded-4xl p-3 hover:bg-gray-500">Projekty</a>
			<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/skills">Zručnosti</a>
			<a class=" rounded-4xl p-3 hover:bg-gray-500" href="/contact">Kontakt</a>
		</div>
	</section>
</header>

<main class="mx-auto min-h-screen px-2 lg:px-6">
	{@render children()}
</main>

<footer>
	<Footer />
</footer>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Gabarito:wght@400..900&display=swap');
	:global(body) {
		background-color: rgba(255, 255, 255, 0.932);
	}
</style>
