<div class="p-8 md:p-16">
<script>
	import { assets } from '$app/paths';
	import { Aperture} from '@lucide/svelte';

	import '../app.css';
	import { page } from '$app/state';

	let { children } = $props();

</script>

<header class="  h-15 justify-center flex border-b-4 border-b-gray-300 bg-gray-400">
	
	<div class="p-3 gabarito-uniquifier space-x-7 text-2xl ">
		<a class="hover:bg-gray-500  rounded-4xl p-3 " href="/">Domov</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/aboutme">O nás</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/websites">Stránky</a>
	
	
	</div>
	<div class="p-2" >	
		<Aperture class='size-10 stroke-2 text-black'/>
	</div>
	<div class="p-3 gabarito-uniquifier space-x-7 text-2xl">
		<a  href="/projects" class=" hover:bg-gray-500  rounded-4xl p-3 " >Projekty</a> 
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/skills">Zručnosti</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/contact">Kontakt</a>
	</div>
</header>


<main>
	{@render children()}
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Gabarito:wght@400..900&display=swap');
	:global(body) {
		background-color: rgba(255, 255, 255, 0.932);
	}
</style>
<section class="text-xs pt-148 "> 


<div class=" bg-gray-300 h-[20px]"> 
	<p class="justify-center items-center flex ">

		<a class="pr-4 hover:text-white" href="/">Domov</a>
		<a class="pr-4 hover:text-white" href="/aboutme">O nás</a>
		<a class=" pr-4 hover:text-white" href="/websites">Stránky</a>
		<a class=" pr-4 hover:text-white " href="/projects"  >Projekty</a> 
		<a class=" pr-4  hover:text-white" href="/skills">Zručnosti</a>
		<a class="pr-4 hover:text-white " href="/contact">Kontakt</a>
			</div>
<div class=" bg-gray-300 h-[20px]"><p class="justify-center items-center flex">@ 2025 Rastislav Šikyňa - Petra Borová</p></div>

</section>
</div>


